---
title: "疊焦技巧 (Focus Stacking)"
aliases: ["疊焦", "焦點堆疊", "Focus Stacking"]
tags:
  - photography
  - techniques
  - macro
created: 2026-11-17
updated: 2026-11-17
sources:
  - "raw/fotobeginner-113-photography-terms.pdf"
  - "raw/cambridge-understanding-depth-of-field.pdf"
---

# 疊焦技巧 (Focus Stacking)

## 一句話核心定義
**疊焦 (Focus Stacking，又稱焦點堆疊)** 是指在相機位置固定下，連續拍攝多張「對焦點由近到遠微幅平移」的照片，再透過後製軟體萃取每張照片中最清晰的切片部位，**融合成一張突破微距光學限制、全域銳利無比相片的進階技法**。

---

## 為什麼需要疊焦？（微距與極端前景的物理死穴）

在 **[[02-optics-and-gear/景深與彌散圓|景深物理學]]** 中，對焦距離越近，景深會呈指數級變淺：
* 當你在 1:1 放大率下拍攝一朵微小的花蕊、昆蟲複眼、或高級珠寶手錶時，即便將光圈縮小至極限的 **f/16 或 f/22**：
  * **物理困境 1**：清晰的景深縱深可能依然**只有短短 0.5 毫米**！花蕊尖端清晰，花瓣根部就糊成一片。
  * **物理困境 2**：超小光圈會引發嚴重的**[[02-optics-and-gear/光學像差與瑕疵|光學繞射 (Diffraction)]]**，讓原本應該清晰的焦點處畫質全體軟化！

---

## 突破物理極限：疊焦工作流程

```text
[固定三腳架與商品] ──► 鏡頭使用最佳銳利度光圈 (如 f/5.6 或 f/8)
      ├── 第 1 張：對焦在物體最前端 (如手錶錶圈前緣)
      ├── 第 2 張：手動旋轉對焦環 1 毫米，對焦在錶盤指針
      ├── 第 3 張：再轉 1 毫米，對焦在手錶時標數字
      └── 第 N 張：對焦在手錶錶背底蓋
               │
               ▼ 匯入 Photoshop / Helicon Focus / Zerene Stacker
[軟體自動對齊] ──► [自動分析每張照片邊緣反差最高 (最銳利) 的區域] ──► [遮罩拼接融合]
               │
               ▼
   【生成全景深作品】：從前到後整支手錶銳利如剃刀，同時享有 f/8 的極致高解像力，無任何光學繞射！
```

---

## 相關概念與延伸閱讀
* [[02-optics-and-gear/景深與彌散圓 (Depth of Field & Circle of Confusion)]] - 對焦距離與極限淺景深
* [[02-optics-and-gear/特殊鏡頭 (Special Lenses)]] - 微距鏡頭特性
* [[02-optics-and-gear/光學像差與瑕疵 (Optical Aberrations)]] - 為什麼不能靠縮到 f/22 解決微距景深
