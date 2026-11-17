# 攝影入門知識庫：LLM Wiki 維護手冊 (AGENTS.md)

本文件是此攝影知識庫的**核心架構規範（Schema）**。所有協助維護本專案的 LLM Agent 必須嚴格遵守本手冊之指引與流程。

---

## 一、 核心哲學與架構

本知識庫基於 **Karpathy LLM Wiki 模式** 構建，致力於打造一個**具有持續演化與複利價值（Compounding）的持久型個人知識庫**。

### 三層架構原則
1. **原始資料層 (`raw/`)**：
   * 收集外部教學文件、PDF、手冊與文章。
   * **不可變（Immutable）**：Agent 僅能讀取與分析，絕不直接修改或覆寫原始檔案。
2. **知識核心層 (`wiki/`)**：
   * 由 LLM Agent 撰寫、提煉、組織與維護的 Markdown 檔案。
   * 包含總目錄 (`index.md`)、維護日誌 (`log.md`) 以及依主題分類的原子化知識卡片。
   * 使用 Obsidian 雙向連結語法相互串聯，保持網狀結構。
3. **規範控制層 (`AGENTS.md`)**：
   * 定義 Agent 的行為守則、語系規則、目錄劃分、卡片格式與 Ingest / Query / Lint 工作流程。

---

## 二、 核心語言與名詞規範（台灣繁中標準）

1. **語系標準**：
   * 一律採用**台灣習慣的繁體中文**（例如：感光元件、全片幅、單眼/無反、景深、散景、暗角、色差/紫邊、後製、直出、向右曝光等）。
2. **中英對照**：
   * 專有名詞、縮寫或關鍵光學/攝影術語，在各頁面**標題與內文首次出現處**必須保留中英對照。
   * 範例：`景深 (Depth of Field / DoF)`、`光圈先決 (Aperture Priority / Av)`、`彌散圓 (Circle of Confusion)`、`快門速度 (Shutter Speed)`。

---

## 三、 原始資料入庫規範（Raw Ingestion Protocol）

當使用者提供新的參考資料時，Agent 須自動執行以下歸檔步驟：
1. **直接上傳 PDF**：
   * 立即儲存至 `raw/` 目錄，並使用乾淨、具備描述性的小寫英文檔名命名（例如：`raw/cambridge-camera-exposure.pdf`）。
2. **提供網址連結 (URL)**：
   * Agent 必須自動透過系統無頭瀏覽器將網頁列印轉換為 PDF（或抓取完整純文字內容），存入 `raw/` 成為不可變原始檔。
   * Windows 命令範例：
     ```powershell
     & "C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" --headless --disable-gpu --run-all-compositor-stages-before-draw --print-to-pdf="raw/<descriptive-name>.pdf" "<URL>"
     ```

---

## 四、 Wiki 目錄架構

知識核心層一律存放於 `wiki/`，目錄規範如下：

```text
wiki/
├── index.md                       # 知識目錄索引（按類別與關鍵概念列出）
├── log.md                         # 變更日誌（Chronological 日誌）
├── 01-exposure/                   # 曝光與相機控制（曝光三要素、模式、測光、直方圖）
├── 02-optics-and-gear/            # 鏡頭、機身與光學（片幅、焦段、透視、景深、像差）
├── 03-lighting-and-accessories/   # 光線、閃光燈與配件（自然光、佈光、濾鏡、腳架）
├── 04-shooting-techniques/        # 拍攝技法與實戰（安全快門、追焦、長曝、構圖、HDR）
├── 05-post-processing/            # 數位暗房與後製（10步工作流、RAW vs JPG、調色）
└── 06-myths-and-comparisons/      # 新手迷思與深度對比（沉澱高價值發問與深度辨析）
```

---

## 五、 筆記撰寫標準（Atomic Notes & Obsidian 規範）

每篇 `wiki/` 筆記皆為**原子化筆記（Atomic Note）**，專注於單一概念或核心主題，並具備高度連結性。

### 1. 雙向連結（Wikilinks）
* 引用其他頁面時，一律使用 Obsidian 相容語法：`[[檔名]]` 或 `[[路徑/檔名|顯示名稱]]`。
* 跨概念應積極連結，例如：在 `人像攝影.md` 中自然連結到 `[[景深與彌散圓]]`、`[[大光圈鏡頭]]`、`[[逆光攝影]]`。

### 2. YAML Frontmatter 格式
每篇 Markdown 筆記開頭必須包含標準元數據：
```yaml
---
title: "頁面完整中文標題 (English Term)"
aliases: ["別名1", "英文縮寫"]
tags:
  - photography
  - 分類標籤 (如 exposure, optics, gear, workflow)
created: 2026-11-17
updated: 2026-11-17
sources:
  - "raw/來源檔名.pdf"
---
```

### 3. 內文結構模組
每篇概念筆記應盡量包含：
1. **一句話核心定義**（適合新手秒懂的白話說明與生活比喻）。
2. **核心原理與關鍵參數**（物理光學、相機運作原理或標準設定級距）。
3. **實戰應用與新手建議**（何時使用、如何設定、常見操作心法）。
4. **相關概念與延伸閱讀**（雙向連結清單）。

---

## 六、 Agent 三大核心操作流程

### 1. Ingest（資料吸收與知識編織）
* **指令**：`ingest raw/<filename>`
* **執行動作**：
  1. 完整閱讀來源檔案，分析並萃取出新的知識點。
  2. 檢查現有 `wiki/` 目錄，判斷應建立哪些新頁面，或在現有頁面中擴充哪些細節。
  3. **編織連結**：在更新的頁面中加入互相參照的雙向連結 (`[[...]]`)。
  4. 若新資料修正或挑戰了舊筆記的觀點，在筆記內標註「觀點演進/爭議點」。
  5. 更新 `wiki/index.md`（加入新頁面或更新摘要）。
  6. 在 `wiki/log.md` 結尾追加一筆紀錄：
     ```markdown
     ## [YYYY-MM-DD] ingest | 來源名稱
     - 建立了：[[xxx]], [[yyy]]
     - 更新了：[[zzz]]
     - 摘要：簡述本次吸收之重點。
     ```

### 2. Query & Compound（查詢與知識沉澱）
* **指令**：使用者提出任何攝影問題或實拍諮詢。
* **執行動作**：
  1. Agent 先查閱 `wiki/index.md` 與相關子目錄筆記。
  2. 綜合 Wiki 現有內容，產出條理清晰、結合實戰的解答，並附上 Wiki 內部頁面參照。
  3. **知識沉澱（Compound）**：若該次問答產出具備高度長期價值之分析（如「35mm vs 50mm 選鏡決策樹」、「RAW vs JPEG 對比」），Agent 應自動將成果寫入 `wiki/06-myths-and-comparisons/`，並回報已歸檔。

### 3. Lint（知識庫健檢與維護）
* **指令**：`lint` 或定期的知識庫健康檢查。
* **執行動作**：
  1. **孤島檢查**：找出沒有任何入站連結（Inbound Links）的孤兒頁面。
  2. **斷鏈檢查**：找出有 `[[頁面]]` 標籤但實體檔案未建立的頁面，列入待建立清單。
  3. **觀點衝突檢查**：比對不同頁面之間是否有互相矛盾的建議。
  4. 在 `wiki/log.md` 紀錄 Lint 報告，並向使用者提示可補強的方向。
