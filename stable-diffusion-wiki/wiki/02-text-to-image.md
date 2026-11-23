# 文字生圖與參數

[回首頁](../README.md) · [上一篇：基本原理](01-basic-principles.md) · [下一篇：採樣與排程](03-sampling.md)

## 要回答的問題

如何描述想要的圖片？哪些設定影響生成？

## 核心概念

以下依據傳統 StableDiffusionPipeline 的參數定義。[S2]

| 參數 | 意義 |
|---|---|
| Prompt | 引導生成內容的文字 |
| Negative Prompt | 引導避開的內容；是否生效取決於 guidance 設定 |
| Steps | 去噪步數；更多步數通常增加耗時 |
| CFG / guidance_scale | 文字引導強度；過高可能降低畫質 |
| generator | 控制隨機數生成，可設定 seed 輔助重現 |

## 教學示例

自訂提示詞：`a cat by a window, watercolor painting`。將它拆成「貓／窗邊／水彩」，練習辨識主體、場景與風格。此例未執行生圖。

## 常見誤解

CFG 不是畫質分數，負面提示詞也不是硬性排除清單。比較設定時，建議固定模型、提示詞、seed 與其他參數，只改一個變因；不要僅憑相同 seed 就假定不同執行環境結果完全相同。

## 自我檢核

想改變畫風應先調整哪一項？想控制修改原圖的幅度，請接著閱讀[Strength](04-image-to-image.md)。

## 來源

S2：[Text-to-image 官方文件](https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion/text2img)，StableDiffusionPipeline.__call__ 的 Parameters。完整紀錄見[來源清單](../sources/references.md)。
