# 圖生圖與 Strength

[回首頁](../README.md) · [上一篇：採樣與排程](03-sampling.md) · [下一篇：ControlNet](05-controlnet.md)

## 要回答的問題

如何以現有圖片為起點？如何調整保留原圖的程度？

## 核心概念

圖生圖接收文字與起始圖片：圖片經過編碼後加入雜訊，再根據文字條件去噪，最後解碼成新圖。[S4]

Strength 影響起點的雜訊程度及有效去噪步數。較低時通常更接近原圖，較高時通常變化更大；它與 Steps 有關，並非單純的圖片混合比例。[S4]

## 教學示例

自訂案例：使用同一張風景照片和「水彩風格」提示詞，比較 Strength 0.3、0.6、0.9。固定其他設定，觀察構圖與風格變化。這是待執行的比較設計，沒有預先假定結果。

## 常見誤解

- Strength 0.6 不代表精確修改 60% 的像素。
- CFG 管文字引導，Strength 管原圖加噪程度，兩者不能互相替代。[S4]

## 自我檢核

若希望保留原圖布局，應先往哪個方向調整 Strength？如果需要更明確的姿勢條件，閱讀[ControlNet](05-controlnet.md)。

## 來源

S4：[Image-to-image 官方教學](https://huggingface.co/docs/diffusers/using-diffusers/img2img)，介紹、Stable Diffusion v1.5、Strength、Guidance scale。完整紀錄見[來源清單](../sources/references.md)。
