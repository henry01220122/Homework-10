# Stable Diffusion 入門 Wiki

從文字生圖到可控生成：供初學者閱讀，也作為 Homework 10 教學 HTML 簡報的知識來源。

## 閱讀順序

| 順序 | 筆記 | 學習問題 | 來源 |
|---|---|---|---|
| 1 | [基本原理](wiki/01-basic-principles.md) | Latent 與去噪是什麼？ | S1、S2 |
| 2 | [文字生圖](wiki/02-text-to-image.md) | Prompt、Steps、CFG 如何影響生成？ | S2 |
| 3 | [採樣與排程](wiki/03-sampling.md) | 每一步如何更新？ | S3 |
| 4 | [圖生圖](wiki/04-image-to-image.md) | 如何利用原圖與 Strength？ | S4 |
| 5 | [ControlNet](wiki/05-controlnet.md) | 如何提供輪廓與姿勢條件？ | S5 |

遇到陌生用語可查閱[中英文名詞表](wiki/glossary.md)。五份原始資料、閱讀範圍與檢查紀錄見[來源清單](sources/references.md)。AI 維護規則見 [AGENTS.md](AGENTS.md)。

## 使用方式

使用支援 Markdown 的編輯器開啟本資料夾，從本頁連結閱讀。所有筆記以相對路徑互連，移動整個資料夾仍可使用。外部資料需網路連線。

本版保存的是五份資料相關章節的中文摘要與來源索引，不是原文全文備份。以傳統 Stable Diffusion 的入門概念為主；不同模型的實作與參數須分別確認。

## 建議簡報對照

| 頁次 | 教學內容 | Wiki 依據 |
|---|---|---|
| 1 | 主題與學習目標 | 本頁 |
| 2–3 | 潛在表示與生成流程 | 基本原理 |
| 4–5 | 提示詞與參數 | 文字生圖 |
| 6 | 步數與採樣方法 | 採樣與排程 |
| 7–8 | 圖生圖與 Strength | 圖生圖 |
| 9–10 | 空間控制與 ControlNet | ControlNet |
| 11 | 概念回顧與自我檢核 | 名詞表、各篇問題 |
| 12 | 參考資料 | 來源清單 |

已依此結構製作 [12 頁 HTML 教學簡報](slides/index.html)。[使用說明](slides/README.md)與[檢查紀錄](slides/validation.md)另附。尚未執行生圖實驗；瀏覽器視覺驗證仍待完成。

## Wiki 建立流程

確認主題與讀者 → 選定五份來源 → 閱讀相關章節 → 寫入主題筆記 → 核對來源與適用範圍 → 檢查內部連結。

來源不足時返回閱讀階段，連結錯誤時返回編輯階段。此流程負責知識整理；模型內部的去噪是另一種迴圈。
