# ControlNet 與空間控制

[回首頁](../README.md) · [上一篇：圖生圖](04-image-to-image.md) · [中英文名詞表](glossary.md)

## 要回答的問題

文字不足以表達精確姿勢或布局時，可以增加什麼資訊？

## 核心概念

ControlNet 為預訓練文字生圖模型加入空間條件。原始研究涵蓋邊緣、深度、分割與人體姿勢等輸入，讓生成更能受到結構資訊引導。[S5]

| 條件 | 提供的結構資訊 |
|---|---|
| 邊緣圖 | 輪廓與線條 |
| 深度圖 | 遠近關係 |
| 姿勢圖 | 人體關節布局 |
| 分割圖 | 區域類別與配置 |

## 教學示例

自訂案例：「正在跳舞的人」搭配指定姿勢圖。文字描述內容，姿勢圖提供結構。這是教學情境，尚未生成圖片。

## 常見誤解

ControlNet 增加控制能力，但不是保證精確複製輸入。一般[圖生圖](04-image-to-image.md)以加噪的原圖表示為起點；ControlNet 另外提供空間條件，兩者也可以組合使用。[S4、S5]

## 自我檢核

要引導動作應選姿勢條件，還是只寫更多形容詞？說明各自提供的資訊。

## 來源

- S5：[ControlNet 原始論文](https://arxiv.org/html/2302.05543v3)，Introduction、Figure 1、§3 Method。
- S4：[Image-to-image](https://huggingface.co/docs/diffusers/using-diffusers/img2img)，介紹。
- 完整紀錄見[來源清單](../sources/references.md)。
