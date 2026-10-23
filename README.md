# FRAME 攝影作品展示與接案 App

手機優先的靜態 PWA，免後端、免框架。

## 先修改

1. 開啟 `index.html`，搜尋 `const CONFIG`，把 `your-email@example.com` 改成你的收件信箱。
2. 搜尋 `const works`，修改作品標題、分類與照片 `src`。建議把自己的照片放在 `photos/`，並用 `photos/xxx.jpg` 當路徑。
3. 修改品牌名稱：HTML 裡的 `FRAME`、`FRAME STUDIO`，以及 `manifest.webmanifest` 的 `name` / `short_name`。
4. 示範照片是外部 Unsplash 圖片，不是攝影師本人的作品；正式營運前請換成自己有權使用的照片。

## 本機測試

用 VS Code 的 Live Server 開啟，或在此資料夾執行 `python3 -m http.server 8000`，再用瀏覽器進入 `http://localhost:8000`。

## GitHub Pages 發布

1. 在 GitHub 建立 public repository，例如 `photo-portfolio`。
2. 上傳本資料夾所有檔案到 repository 根目錄。
3. Settings → Pages → Build and deployment → Deploy from a branch，選 `main` 和 `/ (root)`，按 Save。
4. 等候 GitHub 顯示發布網址，例如 `https://你的帳號.github.io/photo-portfolio/`。
5. iPhone Safari 開啟網址 → 分享 → 加入主畫面。

## 功能與限制

- 首頁、分類作品集、照片大圖、聯絡表單（透過使用者郵件 App 發信）。
- 不含資料庫、付款、預約日曆或自動收件後台。
- 站點介面可離線載入，但外部示範照片離線不保證顯示。
- iPhone 上以 Safari「加入主畫面」使用，不需要 App Store。
