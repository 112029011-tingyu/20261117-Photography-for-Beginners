---
title: "光學像差與瑕疵 (Optical Aberrations)"
aliases: ["光學像差", "色差", "紫邊", "暗角", "鏡頭畸變", "繞射", "Aberrations", "Vignetting", "Distortion"]
tags:
  - photography
  - optics
  - image-quality
created: 2026-11-17
updated: 2026-11-17
sources:
  - "raw/cambridge-understanding-camera-lenses.pdf"
  - "raw/cambridge-understanding-depth-of-field.pdf"
  - "raw/cambridge-digital-photo-editing-workflow.pdf"
  - "raw/fotobeginner-113-photography-terms.pdf"
---

# 光學像差與瑕疵 (Optical Aberrations)

## 一句話核心定義
光學像差是指光線在穿過實體玻璃透鏡組時，無法完美匯聚於同一理想焦點，從而在影像邊緣、高反差輪廓或光暗過渡處產生的**模糊、變色、形變或暗化等物理光學瑕疵**。

---

## 五大常見光學像差與成因

```text
光線經過鏡頭
    ├── 色差/紫邊 (Chromatic Aberration) ──► 不同波長折射率不同 ──► 高反差邊緣浮現紫色/綠色邊緣
    ├── 鏡頭暗角 (Vignetting) ──────────────► 鏡筒邊緣遮光/傾斜進光衰減 ─► 畫面四個角落明顯較暗
    ├── 鏡頭畸變 (Distortion) ──────────────► 廣角桶狀(直線外凸) / 望遠枕狀(直線內縮)
    ├── 鏡頭眩光 (Lens Flare) ──────────────► 強烈直射光在內部鏡片多次反射 ─► 光斑、鬼影與反差驟降
    └── 光學繞射 (Diffraction) ─────────────► 超小光圈(f/16+)時光波產生微觀干涉 ─► 整張照片變軟不銳利
```

### 1. 色差與紫邊 (Chromatic Aberration / Purple Fringing)
* **成因**：紅、綠、藍三種波長的光線穿過透鏡時折射角度略有差異，無法落在同一個點上。
* **現象**：在大光圈全開、或是強烈逆光下（如樹枝映在明亮天空邊緣、太陽逆光人像邊緣），會浮現一圈刺眼的**紫邊 (Purple Fringing)** 或綠邊。
* **解決法**：縮小 1~2 檔光圈；現代相機或後製軟體（如 Lightroom）能一鍵消除色差。

### 2. 鏡頭暗角 (Vignetting / Light Fall-off)
* **成因**：大光圈時邊緣光線斜向射入鏡頭，部分被鏡筒內徑遮蔽（光瞳遮蔽）；或是外掛了太厚的遮光罩/濾鏡。
* **現象**：畫面四個角落的光線亮度明顯比中央暗了一檔左右。
* **解決法**：縮小光圈可大幅消除；後製軟體中啟用「鏡頭設定檔校正」可直接平滑拉亮四角。有時攝影師甚至會刻意保留或後製增加暗角，以聚焦觀者視線。

### 3. 鏡頭幾何畸變 (Geometric Distortion)
* **桶狀變形 (Barrel Distortion)**：常見於廣角端（如 16mm~24mm），直線向外彎曲膨脹（中間外凸）。
* **枕狀變形 (Pincushion Distortion)**：常見於長焦端（如 135mm~200mm），直線向內塌陷凹陷。
* **解決法**：後製軟體網格拉正；建築攝影中需格外重視，避免高樓直線歪斜。

### 4. 鏡頭眩光與鬼影 (Lens Flare & Ghosting)
* **成因**：強烈直射光源（如太陽或強力路燈）直射鏡頭前組鏡片，在鏡片群之間多次折射與反射。
* **現象**：畫面上出現多邊形光斑、光霧，整張照片的**對比度與飽和度瞬間劇降（畫面發灰發白）**。
* **解決法**：裝上**[[03-lighting-and-accessories/實用輔助器材|鏡頭遮光罩 (Lens Hood)]]**、微調拍攝角度避開直射光；有時逆光小清新風格會刻意善用眩光營造夢幻氛圍。

### 5. 光學繞射 (Diffraction)：超小光圈的死穴
* **成因**：光圈縮到極小（如 f/16, f/22, f/32）時，光波通過微小針孔邊緣產生繞射干涉，使本該匯聚的點發散為「艾里斑 (Airy Disk)」。
* **迷思打破**：**不要以為光圈越小畫質越好！** 超小光圈雖然景深極深，但繞射會讓全片幅像素點糊成一片，整張照片銳利度嚴重衰退。風景攝影最佳銳利度通常落在 **f/5.6 ~ f/11**。

---

## 相關概念與延伸閱讀
* [[01-exposure/光圈 (Aperture)]] - 光圈開大與收小時像差的消長
* [[03-lighting-and-accessories/實用輔助器材]] - 遮光罩預防眩光的作用
* [[05-post-processing/鏡頭數位校正]] - 數位暗房如何自動修正色差與幾何變形
