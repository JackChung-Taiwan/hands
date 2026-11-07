# 手勢魔法 Hand Magic FX

乾淨的全畫面手勢特效。移除城堡、敵人、計分、生命與倒數，讓特效跟隨手的位置。

體驗：https://jackchung-taiwan.github.io/hands/

| 手勢 | 特效 |
|---|---|
| 握拳 | 爆裂火花 |
| 1 指 | 流星光筆 |
| 2 指 | 雷電雙刃 |
| 3 指 | 冰晶旋風 |
| 4 指 | 花瓣飛舞 |
| 5 指 | 奧術光環 |
| OK | 星河漩渦 |
| 讚（拇指） | 烈焰升騰 |
| 搖滾（食指＋小指） | 電音波紋 |
| 小指 | 泡泡精靈 |
| 雙掌 | 彩虹傳送門 |
| 雙拳 | 超新星 |
| 雙 1 指 | 電光連線 |
| 雙 OK | 愛心星塵 |

左右手使用不同配色。保持手勢會持續施放；手勢穩定約 170ms 才切換，單手施放間隔 620ms，雙手組合間隔 1100ms。數字指伸出的手指總數；特殊手勢優先於數量辨識。建議 1～4 指使用食指起依序伸展。

開啟攝影機後手勢表自動收起。可切換黑底、全螢幕與特效密度。H 隱藏介面、Esc 恢復，右下角選單也可恢復。數字 0～9 或手勢表按鈕可預覽特效。

單一 index.html，不需要建置。需要 HTTPS 或 localhost、攝影機授權，以及 jsDelivr / Google 模型網路連線。影像在瀏覽器本機辨識，程式沒有影像上傳功能。攝影機關閉時停止所有影像軌道。

內建 Canvas 粒子搭配可選 PixelFX 火花、冰霜、雷電、奧術特效；PixelFX 載入失敗不會阻擋鏡頭及內建特效。MediaPipe Tasks Vision 固定版本 0.10.32，WASM 使用相同版本。粒子與特效數量有上限。

## 驗證

已檢查 JavaScript 語法，並以模擬 Canvas/DOM 驗證 14 種內建特效可建立、逐幀繪製與到期移除。尚需實際攝影機驗證手勢準確率、行動裝置效能及 CDN 載入。

## 第三方授權

- [PixelFX](https://github.com/patch-gg/pixelfx)：MIT，參閱其 LICENSE 與 NOTICE.md。
- MediaPipe Tasks Vision：Apache-2.0。

既有 .github/workflows/deploy.yml 負責 GitHub Pages 部署。
