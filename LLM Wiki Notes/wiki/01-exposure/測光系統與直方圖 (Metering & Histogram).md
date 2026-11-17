---
title: "測光系統與直方圖 (Metering & Histogram)"
aliases: ["測光模式", "直方圖", "Metering", "Histogram", "ETTR", "向右曝光"]
tags:
  - photography
  - exposure
  - camera-operation
created: 2026-11-17
updated: 2026-11-17
sources:
  - "raw/cambridge-camera-exposure.pdf"
  - "raw/fotobeginner-113-photography-terms.pdf"
---

# 測光系統與直方圖 (Metering & Histogram)

## 一句話核心定義
相機內建的**測光錶 (Light Meter)** 負責評估現場光影並決定「正常曝光」基準；而**直方圖 (Histogram)** 則是客觀檢驗照片明暗分佈、防止「死白」或「死黑」的最佳數位工具。

---

## 一、 相機三大測光模式 (Metering Modes)

數位相機透過鏡頭測光（TTL，Through-The-Lens），相機將世界預設為 **18% 中性灰（18% Neutral Gray）**。常見測光模式包含：

| 測光模式 | 圖示與別名 | 測光範圍與權重 | 適用場景 |
| :--- | :--- | :--- | :--- |
| **全區測光 / 權衡測光 (Evaluative / Matrix)** | 圓形帶圓點 | 將整個畫面分割為數十至數百個區域，綜合主體對焦點做加權平均 | **90% 日常拍攝預設**：風景、街拍、日常紀錄 |
| **中央重點測光 (Center-weighted)** | 括弧帶大圓 | 測量整個畫面，但給予中央約 60%~80% 區域最高權重 | 傳統紀實、主體明確位居中央的人像 |
| **點測光 (Spot Metering)** | 單一小圓點 | 僅測量畫面中央（或對焦點連動）極小區域（約 1%~3% 面積） | **極端高反差場景**：舞台聚光燈下人物、大逆光人像臉部、微距昆蟲 |

---

## 二、 直方圖解讀：科學評估曝光的靈魂之窗

相機螢幕在烈日下看容易誤判亮度，唯有 **直方圖 (Histogram)** 絕不说謊。直方圖橫軸為亮度（左黑右白），縱軸為像素數量：

```text
像素數量 (Pixels)
   ▲
   │        ┌─┐      
   │     ┌──┘ └──┐   
   │  ┌──┘       └──┐
───┴──┴─────────────┴──► 亮度 (Brightness)
   0 (純黑/暗部)    255 (純白/亮部)
  【死黑/欠曝】     【死白/過曝】
```

### 三種典型直方圖型態
1. **正常曝光 (Balanced Exposure)**：像素主要分佈在中間調，兩側邊界自然落下，未頂到最左或最右牆壁。
2. **曝光不足 (Under-Exposed)**：大量波峰擠壓在最左側（0 處撞牆），產生「**死黑 (Clipped Shadows)**」，暗部細節完全喪失為純黑噪點。
3. **過度曝光 (Over-Exposed / Blown-out)**：大量波峰堆積在最右側（255 處撞牆），產生「**死白 (Clipped Highlights)**」，天空或皮膚泛白無任何數位資訊，後製無法挽救。

---

## 三、 進階技巧：向右曝光 (Expose to the Right / ETTR)

* **原理**：數位相機感光元件在最明亮的一檔（右側）能記錄下最多的色階資訊與動態範圍（高訊噪比）。
* **操作法**：在拍攝 RAW 檔時，適度增加曝光，讓直方圖的波峰盡可能靠近右側邊界，但**絕對不可撞牆溢出（避免高光死白）**。在後製時再將整體曝光拉回，可獲得極致純淨、無暗部雜訊的高畫質作品。

---

## 相關概念與延伸閱讀
* [[曝光三要素 (Exposure Triangle)]] - 曝光控制基礎
* [[曝光補償 (Exposure Compensation)]] - 修正測光被雪景或黑夜欺騙的關鍵旋鈕
* [[05-post-processing/曝光微調與高光陰影還原]] - 數位暗房如何利用直方圖拉回高光
* [[05-post-processing/RAW vs JPEG 深度解析 (RAW vs JPEG Format)|RAW vs JPEG 深度解析]] - 為什麼 ETTR 必須搭配 RAW 檔
