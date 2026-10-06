# Games

單檔網頁遊戲合集（landing page + 各遊戲子頁）。

**線上位址**：https://lsisan1212.github.io/Games/
**遊戲子頁**：https://lsisan1212.github.io/Games/Rummuku.html

## 結構

| 檔案 | 用途 |
|---|---|
| `index.html` | Landing page：卡片入口、搜尋、4 套主題（記住選擇） |
| `games.json` | 遊戲清單 manifest（唯一要改嘅檔） |
| `Rummuku.html` | Rummikub 拉密（2–4 人、計時、出牌提示） |
| `.nojekyll` | 關 Jekyll |

## 收錄

| 檔案 | 遊戲 | 說明 |
|---|---|---|
| `Rummuku.html` | Rummikub 拉密 | 2–4 人對戰、計時、出牌提示、牌池顯示 |

## 加新遊戲（3 步）

1. 把單檔 HTML 丟落根目錄，例如 `ChessTrainer.html`
2. 喺 `games.json` 嘅 `games` 陣列加一項：

```json
{
  "file": "ChessTrainer.html",
  "title": "Chess Trainer",
  "titleZh": "西洋棋",
  "desc": "一句描述。",
  "emoji": "♟️",
  "accent": "#7F77DD",
  "tags": ["對戰", "益智"]
}
```

3. `git add -A && git commit -m "add: ChessTrainer" && git push` → 約 30–60 秒生效

> 漏咗第 2 步都會自動顯示（landing page 會經 GitHub API 偵測根目錄 `*.html` 並用檔名推導標題），但補上 JSON 才會有中文名／描述／標籤／強調色。

## 本地使用

```bash
open index.html      # landing page
open Rummuku.html    # 直接開遊戲
```

## 特點

- 全部單檔、零外部 CDN／框架／字型，`file://` 都跑得（landing page 有內建 fallback 清單）
- 主題（深色／淺色／海洋／日落）存 `localStorage`

## 部署

GitHub Pages（`main` 分支根目錄），已加 `.nojekyll`。
