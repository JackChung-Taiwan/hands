# 雙手魔法守護者 Hand Magic

這是一個使用 MediaPipe Hand Landmarker 與 [PixelFX](https://github.com/patch-gg/pixelfx) 的兒童體感魔法遊戲。

## 遊戲網址

啟用 GitHub Pages 後： https://jackchung-taiwan.github.io/hands/

## 操作方法

| 手勢 | 技能 | 鍵盤 |
|---|---|---|
| 左手張掌橫揮 | 冰霜衝擊 | Q |
| 右手張掌橫揮 | 雷霆之擊 | E |
| 左手握拳 | 爆裂火花 | A |
| 右手握拳 | 奧術結界 | D |

每局 60 秒，有怪物、分數、連擊與 3 點生命。也能直接點擊網頁的魔法按鈕操作。

本專案為**單一 index.html 靜態網頁**，透過 CDN 載入 MediaPipe 與 PixelFX 模組，不需要建置或安裝套件。攝影機必須在 HTTPS 或 localhost 環境使用，並由使用者主動授權。攝影機影像在瀏覽器本機進行分析，沒有自訂的影像上傳功能；MediaPipe 套件仍可能收集效能與使用指標，詳情參見其隱私公告。

## GitHub Pages

前往 **Settings → Pages → Build and deployment → Source → GitHub Actions**，儲存後於 Actions 頁面重新執行 **Deploy Hands Magic Game**，或推送一筆新提交以啟動部署。部署成功後，開啟 https://jackchung-taiwan.github.io/hands/ 。

## 第三方程式及授權

- PixelFX：MIT， https://github.com/patch-gg/pixelfx （詳見其 [LICENSE](https://github.com/patch-gg/pixelfx/blob/main/LICENSE)、[NOTICE](https://github.com/patch-gg/pixelfx/blob/main/NOTICE.md)）
- MediaPipe Tasks Vision：Apache-2.0， https://www.npmjs.com/package/@mediapipe/tasks-vision

注意：首次進入必須能連線到 Google 模型儲存位置及 jsDelivr CDN。正式課程請先用實際網路攝影機測試動作門檻與裝置效能。
