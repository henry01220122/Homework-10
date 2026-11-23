# 中英文名詞表

[回首頁](../README.md)

本表為閱讀導航，定義的適用範圍與來源請見對應筆記。

| 英文 | 中文與簡意 | 詳細筆記 |
|---|---|---|
| Latent representation | 潛在表示：壓縮後的學習特徵 | [基本原理](01-basic-principles.md) |
| Denoising | 去噪：逐步更新帶噪表示 | [基本原理](01-basic-principles.md) |
| VAE | 變分自編碼器：在圖像與潛在表示間編解碼 | [基本原理](01-basic-principles.md) |
| U-Net | 此 pipeline 使用的去噪網路 | [基本原理](01-basic-principles.md) |
| Prompt | 提示詞 | [文字生圖](02-text-to-image.md) |
| Negative Prompt | 負面提示詞 | [文字生圖](02-text-to-image.md) |
| CFG | Classifier-Free Guidance，無分類器引導 | [文字生圖](02-text-to-image.md) |
| Seed | 隨機種子 | [文字生圖](02-text-to-image.md) |
| Steps | 去噪步數 | [文字生圖](02-text-to-image.md) |
| Sampler | 採樣方法 | [採樣與排程](03-sampling.md) |
| Scheduler | 排程器；在 Diffusers 中也涵蓋更新方法 | [採樣與排程](03-sampling.md) |
| img2img | 圖生圖 | [圖生圖](04-image-to-image.md) |
| Strength | 圖生圖的加噪強度設定 | [圖生圖](04-image-to-image.md) |
| ControlNet | 加入空間條件的控制網路 | [ControlNet](05-controlnet.md) |

## 作業用語

- **Ingest**：本專案指閱讀來源、摘取重點、寫入筆記並建立出處關聯。
- **Wiki**：以索引、連結與來源組織的知識筆記。
- **Graph**：資料取得、整理、檢查與輸出的節點及連線。
- **Loop**：檢查未通過時返回相關步驟修正，並設停止條件。

以上作業用語是本專案的操作定義，與模型內部的去噪步驟分開。
