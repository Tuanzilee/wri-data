# 寫作範本銀行 · Writing Template Bank

一個給自己用的寫作範本管理工具,專為考試寫作練習設計。三本銀行 + 練習模式,放上 GitHub Pages 後就能在任何裝置開啟。

## 功能

- **翻譯句型庫** — 中翻英常用句型 + 中英例句對照
- **英文作文庫** — 開頭、段落、轉折、結尾模板
- **國文素材庫** — 破題模板、名句、人物事件素材
- **練習模式** — 隨機抽卡,翻面看答案,自動依答對與否升降難度
- **A/B/C 難度分級** — 答對自動升級、答錯自動降級
- **匯出/匯入 JSON** — 跨裝置同步 + 備份
- **資料儲存於 localStorage** — 完全離線、無需後端

## 部署到 GitHub Pages(三步驟)

### 1. 建立 repo
到 [github.com/new](https://github.com/new) 建一個新的 repository(可以是 public 或 private,Pages 都支援)。

### 2. 上傳 index.html
把 `index.html` 上傳到 repo 根目錄。可以用網頁介面拖拉、或用 git:

```bash
git clone https://github.com/你的帳號/repo名稱.git
cd repo名稱
# 把 index.html 複製進來
git add index.html
git commit -m "Initial template bank"
git push
```

### 3. 開啟 Pages
進到 repo → Settings → Pages → Source 選 `Deploy from a branch` → Branch 選 `main`(或 `master`)→ 資料夾選 `/ (root)` → Save。

等 1–2 分鐘,你的網站就會在 `https://你的帳號.github.io/repo名稱/` 上線了。

## 使用建議

- **加入 iPad/手機主畫面** — Safari 開啟 → 分享 → 加入主畫面,用起來像 App
- **每週匯出一次 JSON 備份** — 點左上角的 ↓ 按鈕,存到雲端硬碟
- **練習模式預設只練 B+C** — 把時間花在不熟的項目上,別重複練已經會的
- **答對會自動升級難度,答錯會降級** — 不需要手動維護分類

## 資料安全

- 所有資料存在你的瀏覽器本機(localStorage),不會上傳任何雲端
- 換裝置請用「匯出 JSON」備份,在新裝置「匯入 JSON」還原
- 清除瀏覽器資料會清空銀行,務必先備份

## 客製化

整個 app 是單一 HTML 檔,所有 CSS 和 JS 都在裡面。要改顏色、字體、新增分類,直接編輯 `index.html` 上方的 `:root` CSS 變數和對應的 HTML 區塊就行。
