# Games

單檔網頁遊戲合集。目前收錄：**Rummikub（拉密）**。

**線上位址**：https://lsisan1212.github.io/Games/

## 收錄

| 檔案 | 遊戲 | 說明 |
|---|---|---|
| `index.html` | Rummikub 拉密 | 2–4 人、計時、出牌提示、牌池顯示 |

## 特點

- 純 HTML + CSS + JS 單一檔案，無任何外部 CDN / 框架 / 字型
- 雙擊 `index.html` 即可玩（`file://` 都正常）

## 本地使用

```bash
open index.html
```

## 部署

GitHub Pages（`main` 分支根目錄），已加 `.nojekyll` 避開 Jekyll 處理。
改完內容 → `git push` → Pages 約 30–60 秒後重新建置。

之後要加新遊戲：丟一個單檔 HTML 落根目錄，再喺上表加一行。
