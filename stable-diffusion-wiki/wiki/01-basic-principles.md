# 基本原理

[回首頁](../README.md) · [下一篇：文字生圖](02-text-to-image.md)

## 要回答的問題

為什麼要使用潛在空間？文字如何參與生成？

## 核心概念

Latent Diffusion 把主要生成運算放在壓縮後的潛在表示中，以降低直接處理像素的計算負擔。編碼器將影像轉成潛在表示，解碼器將表示還原為可見圖片；文字等條件可透過 cross-attention 引導生成。[S1]

傳統 StableDiffusionPipeline 使用文字編碼器、U-Net、Scheduler 與 VAE。文字生圖從隨機潛在雜訊開始，配合文字條件反覆更新，再由 VAE 解碼；並非每次文字生圖都要先輸入一張照片。[S2]

## 常見誤解

- Latent 是學得的特徵表示，不等於縮小尺寸的照片。
- 此處的 U-Net 架構說明限於所引用的 pipeline，不代表所有 Stable Diffusion 版本。

## 教學示例與自我檢核

可用「在精簡表示中生成，再轉成圖片」作為口頭說明。問題：文字生圖與圖生圖的起點有何不同？請閱讀[圖生圖](04-image-to-image.md)後回答。

## 來源

- S1：[Latent Diffusion 論文](https://arxiv.org/html/2112.10752v2)，§3.1–3.3。
- S2：[StableDiffusionPipeline](https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion/text2img)，元件與呼叫參數。
- 完整資料見[來源清單](../sources/references.md)。
