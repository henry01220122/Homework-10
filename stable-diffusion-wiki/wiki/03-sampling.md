# 採樣與排程

[回首頁](../README.md) · [上一篇：文字生圖](02-text-to-image.md) · [下一篇：圖生圖](04-image-to-image.md)

## 要回答的問題

為什麼相同步數，仍可能產生不同結果？

## 核心概念

Diffusers 的 Scheduler 管理去噪更新與時間步安排。方法不同，速度與生成品質的取捨也可能不同。文件建議先使用模型預設排程器，再依需求改用相容設定。[S3]

| 概念 | 解釋 |
|---|---|
| Steps | 更新過程的步數 |
| 採樣更新方法 | 如何利用模型輸出更新潛在表示 |
| Noise / timestep schedule | 各步的雜訊等級或時間點安排 |

在 Diffusers 中，Scheduler 可涵蓋更新方法與排程；其他介面可能將 Sampler 與 Scheduler 分成不同欄位，不宜只看名稱判定完全相同。[S3]

## 教學示例

可把 Steps 比喻成「走幾步」，更新方法比喻成「如何走」。這只是概念比喻，不是數學定義。

## 常見誤解

不能把任意 Scheduler 套到任意模型；需要確認相容性。也不能只依步數比較不同方法的效果。

## 自我檢核

若要比較兩種方法，哪些設定應固定？可回看[文字生圖](02-text-to-image.md)的比較建議。

## 來源

S3：[Schedulers 官方文件](https://huggingface.co/docs/diffusers/using-diffusers/schedulers)，Choosing a scheduler、Loading schedulers、Timestep schedules。完整紀錄見[來源清單](../sources/references.md)。
