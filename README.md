# Rummuku

單檔網頁版 **Rummikub**（拉密）—— 零依賴、零 build、離線可用。

**線上位址**：https://lsisan1212.github.io/Rummuku/

## 特點

- 純 HTML + CSS + JS 單一檔案，無任何外部 CDN / 框架 / 字型
- 雙擊 `index.html` 即可玩（`file://` 都正常）
- 支援 2–4 人、計時、出牌提示、牌池顯示

## 本地使用

```bash
open index.html
```

## 部署

GitHub Pages（`main` 分支根目錄），已加 `.nojekyll` 避開 Jekyll 處理。
改完 `index.html` → `git push` → Pages 約 30–60 秒後重新建置。
