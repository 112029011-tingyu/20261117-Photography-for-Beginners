# 知識庫維護日誌 (Log)

本文件以時間倒序（或正規時間軸順序）記錄知識庫的所有操作，包含 Ingest（資料吸收）、Query（深度問答沉澱）與 Lint（健康檢查）。

---

## [2026-11-17] init | 專案初始化與結構建立
- **操作類型**：初始化 (Initialization)
- **完成項目**：
  - 建立知識庫規則手冊 `AGENTS.md`。
  - 建立原始資料夾 `raw/` 並妥善安置 5 份種子教材 PDF。
  - 建立 6 大領域知識分類目錄 (`01-exposure` 至 `06-myths-and-comparisons`)。
  - 建立總目錄索引 `wiki/index.md` 與日誌 `wiki/log.md`。
- **後續步驟**：準備啟動首波核心資料 Ingest，萃取曝光、鏡頭光學與後製工作流等原子筆記。


## [2026-11-17] ingest | raw/cambridge-camera-exposure.pdf
- **操作類型**：資料吸收 (Ingest)
- **建立了**：
  - [[01-exposure/曝光三要素 (Exposure Triangle)]]
  - [[01-exposure/光圈 (Aperture)]]
  - [[01-exposure/快門速度 (Shutter Speed)]]
  - [[01-exposure/感光度 (ISO)]]
  - [[01-exposure/曝光級數 (Exposure Stops)]]
  - [[01-exposure/相機拍攝模式 (Camera Modes)]]
- **更新了**：
  - [[wiki/index.md]]
- **摘要**：完整吸收了 Cambridge in Colour 曝光核心手冊，將曝光三要素拆解為 5 篇原子化核心筆記，並建構了完整的相機曝光模式（PASMB）解析卡片，完成全站首批雙向網狀連結與雨桶比喻模型。


## [2026-11-17] ingest | 全面吸收剩餘 4 份核心教材
- **來源清單**：
  - `raw/cambridge-understanding-camera-lenses.pdf`
  - `raw/cambridge-understanding-depth-of-field.pdf`
  - `raw/cambridge-digital-photo-editing-workflow.pdf`
  - `raw/fotobeginner-113-photography-terms.pdf`
- **操作類型**：批量資料吸收與全域編織 (Batch Ingest & Synthesis)
- **建立了**：
  - `01-exposure/`：[[01-exposure/測光系統與直方圖 (Metering & Histogram)]]、[[01-exposure/曝光補償 (Exposure Compensation)]]
  - `02-optics-and-gear/`：[[02-optics-and-gear/感光元件與片幅 (Sensor & Crop Factor)]]、[[02-optics-and-gear/單眼與無反 (DSLR vs Mirrorless)]]、[[02-optics-and-gear/焦距與視角 (Focal Length & Angle of View)]]、[[02-optics-and-gear/透視感與空間壓縮 (Perspective & Compression)]]、[[02-optics-and-gear/景深與彌散圓 (Depth of Field & Circle of Confusion)]]、[[02-optics-and-gear/散景 (Bokeh)]]、[[02-optics-and-gear/定焦鏡與變焦鏡 (Prime vs Zoom)]]、[[02-optics-and-gear/光學像差與瑕疵 (Optical Aberrations)]]、[[02-optics-and-gear/特殊鏡頭 (Special Lenses)]]
  - `03-lighting-and-accessories/`：[[03-lighting-and-accessories/自然光與光質 (Ambient Light & Quality)]]、[[03-lighting-and-accessories/基礎人像佈光 (Basic Portrait Lighting)]]、[[03-lighting-and-accessories/閃光燈與同步 (Flash & Synchronization)]]、[[03-lighting-and-accessories/離機閃與控光配件 (OCF & Modifiers)]]、[[03-lighting-and-accessories/攝影濾鏡 (Photography Filters)]]、[[03-lighting-and-accessories/實用輔助器材 (Useful Accessories)]]
  - `04-shooting-techniques/`：[[04-shooting-techniques/安全快門與防震 (Safe Shutter Speed & Stabilization)]]、[[04-shooting-techniques/自動對焦系統 (Autofocus Modes & BBF)]]、[[04-shooting-techniques/速度動態技法 (Motion Techniques)]]、[[04-shooting-techniques/構圖原則與畫面比例 (Composition & Aspect Ratio)]]、[[04-shooting-techniques/高動態範圍與包圍曝光 (Bracketing & HDR)]]、[[04-shooting-techniques/疊焦技巧 (Focus Stacking)]]
  - `05-post-processing/`：[[05-post-processing/數位後製標準十步工作流 (10-Step Workflow)]]、[[05-post-processing/白平衡與色溫校正 (White Balance & Color Temperature)]]、[[05-post-processing/曝光微調與高光陰影還原 (Exposure & Dynamic Range Recovery)]]、[[05-post-processing/降噪與銳化平衡 (Noise Reduction vs Sharpening)]]、[[05-post-processing/鏡頭數位校正 (Lens Corrections)]]、[[05-post-processing/對比度、階調與色調曲線 (Contrast, Levels & Curves)]]、[[05-post-processing/裁切構圖與色彩微調 (Framing & Color Refinements)]]、[[05-post-processing/影像縮放與輸出銳化 (Resizing & Output Sharpening)]]、[[05-post-processing/RAW vs JPEG 深度解析 (RAW vs JPEG Format)]]
  - `06-myths-and-comparisons/`：[[06-myths-and-comparisons/迷思：焦距到底會不會改變景深？]]、[[06-myths-and-comparisons/迷思：高像素等於高畫質？聞相迷思 (Pixel Peeping)]]、[[06-myths-and-comparisons/迷思：後製執相就是作假？]]、[[06-myths-and-comparisons/比較：定焦鏡練習走位 vs 變焦鏡靈活性 (Prime vs Zoom)]]
- **更新了**：
  - [[wiki/index.md]]
- **摘要**：全量消化剩餘 4 份種子教材，建立共 33 篇具備高密度 Obsidian 雙向連結之原子化筆記，全景涵蓋相機控制、鏡頭光學物理、閃燈佈光與配件、速度動態技法、數位暗房 10 步工作流、以及四大攝影界經典迷思與決策樹。
