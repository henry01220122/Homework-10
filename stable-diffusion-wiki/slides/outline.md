# 簡報大綱與來源對照

## 生成前檢查

範圍採用 Wiki 的傳統 StableDiffusionPipeline；不加入 SD3 或 Turbo 的參數建議。所有圖形為概念示意，沒有使用或聲稱真實生圖實驗。

| 頁 | 主題 | Wiki | 來源 |
|---|---|---|---|
| 1 | 主題與學習目標 | README.md | 編輯規劃 |
| 2 | 潛在表示 | wiki/01-basic-principles.md | S1 |
| 3 | 文字生圖流程 | wiki/01-basic-principles.md | S1、S2 |
| 4 | Prompt 的構成 | wiki/02-text-to-image.md | S2；自訂示例 |
| 5 | Steps、CFG 與 Seed | wiki/02-text-to-image.md | S2 |
| 6 | 採樣與排程 | wiki/03-sampling.md | S3 |
| 7 | 圖生圖流程 | wiki/04-image-to-image.md | S4 |
| 8 | Strength 概念 | wiki/04-image-to-image.md | S4 |
| 9 | ControlNet 空間條件 | wiki/05-controlnet.md | S5 |
| 10 | 生成方式的選擇 | wiki/04-image-to-image.md、wiki/05-controlnet.md | S2、S4、S5；教學整理 |
| 11 | 自我檢核 | 上述五篇 | S2、S4、S5 |
| 12 | 五份參考資料 | sources/references.md | S1–S5 |

內容檢查條件：每頁有可追溯來源；CFG 不寫成畫質分數；Strength 不寫成像素修改百分比；Seed 不保證跨環境一致；ControlNet 不宣稱百分之百控制。此五項在大綱階段先確認，避免完成 HTML 才修改概念。
