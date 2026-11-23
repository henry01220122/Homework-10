# 來源清單與閱讀紀錄

[回首頁](../README.md)

閱讀與整理日期：2026-11-23（Asia/Taipei）。本次以相關章節的重點摘要方式 ingest 五份資料；未保存原文全文，也不將章節閱讀記為全文精讀。Hugging Face 文件為持續更新頁面，下次修改時須重查。

## S1 Latent Diffusion

- 標題：High-Resolution Image Synthesis with Latent Diffusion Models。
- 作者：Robin Rombach、Andreas Blattmann、Dominik Lorenz、Patrick Esser、Björn Ommer。
- 年份與版本：CVPR 2022；arXiv 2112.10752 v2。
- [原始來源](https://arxiv.org/html/2112.10752v2)
- 閱讀範圍：摘要、方法 §3.1–3.3；重點為影像壓縮、潛在擴散、條件機制。
- 產出：[基本原理](../wiki/01-basic-principles.md)。不以此來源推論所有後續 SD 版本。

## S2 Stable Diffusion Text-to-image

- 作者／維護者：Hugging Face Diffusers 團隊與貢獻者。
- 類型：程式庫官方 API 文件。
- [原始來源](https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion/text2img)
- 閱讀範圍：StableDiffusionPipeline 元件與 __call__ Parameters。
- 產出：[文字生圖](../wiki/02-text-to-image.md)、[基本原理](../wiki/01-basic-principles.md)。參數說明限於所列 pipeline，不把預設值當成通用最佳值。

## S3 Schedulers

- 作者／維護者：Hugging Face Diffusers 團隊與貢獻者。
- 類型：程式庫官方指南。
- [原始來源](https://huggingface.co/docs/diffusers/using-diffusers/schedulers)
- 閱讀範圍：Choosing a scheduler、Loading schedulers、Timestep schedules。
- 產出：[採樣與排程](../wiki/03-sampling.md)。著重更新方法與相容性，不提供未實測的排行榜。

## S4 Image-to-image

- 作者／維護者：Hugging Face Diffusers 團隊與貢獻者。
- 類型：程式庫官方教學。
- [原始來源](https://huggingface.co/docs/diffusers/using-diffusers/img2img)
- 閱讀範圍：介紹、Stable Diffusion v1.5、Strength、Guidance scale。
- 產出：[圖生圖](../wiki/04-image-to-image.md)。不將文件中的其他模型架構混入 SD 基礎說明。

## S5 ControlNet

- 標題：Adding Conditional Control to Text-to-Image Diffusion Models。
- 作者：Lvmin Zhang、Anyi Rao、Maneesh Agrawala。
- 年份與版本：2023；arXiv 2302.05543 v3。
- [原始來源](https://arxiv.org/html/2302.05543v3)
- 閱讀範圍：摘要、Introduction、Figure 1、§3 Method。
- 產出：[ControlNet](../wiki/05-controlnet.md)。著重空間條件，不把論文結果當成本專案實測。

## 實際整理紀錄

1. 依先前討論確定新手導向的五個主題。
2. 開啟五份來源核對相關內容，為每篇建立來源編號與筆記。
3. 編輯時納入範圍限制：CFG 不等於畫質分數、Strength 不等於修改百分比、Scheduler 需相容、U-Net 說明不能套用所有版本。
4. 所有自訂生圖案例標記為示例或待執行設計。

本紀錄描述 Wiki 建立工作；未執行 Stable Diffusion 生圖、HTML 顯示測試或整份作業的反思實驗。

## 結構檢查

2026-11-23 執行結構檢查：

- 九個 Markdown 檔案齊全，均有標題。
- 54 個本機相對連結全部指向存在的檔案。
- 五篇主題筆記均含問題、核心概念、常見誤解與來源欄位。
- 五份外部來源已於整理時開啟核對；本機連結檢查不代表外部網址永久有效。
- 此輪結構檢查未發現失效本機連結；沒有虛構失敗或重試紀錄。
