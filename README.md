# 銀河遊戲大廳 · Galaxy Game Arcade

20 款經典街機遊戲，全部以純 HTML + JavaScript 實現，**無任何外部依賴**，開啟即玩。

![preview](1.jpg)

---

## 遊戲列表

| 遊戲 | 分類 | 玩法 |
|---|---|---|
| 🐍 **貪吃蛇** · 霓光版 | 休閒 | 方向鍵控制蛇吃食物，越吃越長 |
| 🐝 **小蜜蜂 豪華版** | 射擊 | 經典 Galaga 縱向射擊，關卡推進 |
| 🧱 **俄羅斯方塊 豪華版** | 消除 | 標準方塊消除，含暫存區與預覽 |
| 🏓 **打磚塊 豪華版** | 街機 | 反彈擊碎所有磚塊，多重道具 |
| 🧠 **記憶翻牌 豪華版** | 益智 | 配對翻牌，考驗記憶力 |
| 🚀 **太空大戰** | 射擊 | 橫向太空射擊，閃避敵機 |
| 🔥 **火鳳凰** | 射擊 | 鳳凰主題縱向射擊 |
| ✈️ **雷電飛機 Remastered** | 射擊 | 縱向彈幕射擊，經典雷電玩法 |
| 🃏 **21 點 豪華版** | 卡牌 | 莊家對戰，Blackjack 規則 |
| 🪙 **金樸克** | 卡牌 | 街機 Video Poker 撲克 |
| ⚫ **五子棋** | 棋類 | 人機對弈，先連五子者勝 |
| 💣 **炸彈人** | 動作 | 迷宮放置炸彈，爆破敵人 |
| 🛡️ **坦克大戰 豪華版** | 動作 | Battle City 風格坦克對戰 |
| 🦖 **恐龍快跑** | 跑酷 | Chrome 恐龍跳躍躲避障礙 |
| ⚪ **黑白棋 Reversi** | 棋類 | 翻轉對手棋子 |
| ♟️ **中國象棋** | 棋類 | 人機對弈，完整象棋規則 |
| 🐦 **Flappy Bird** | 休閒 | 經典點擊飛越管道 |
| 💥 **掃雷** | 益智 | 經典邏輯推理踩雷 |
| 🖱️ **點擊大師** | 放置 | 點擊升級，放置累積 |
| 🥊 **快打旋風 街頭對決** | 格鬥 | 1v1 格鬥，必殺技系統 |

---

## 技術特點

- **100% 純前端** — 僅 HTML / CSS / JavaScript，無框架、無套件
- **17 款 Canvas 2D 渲染**，使用 `requestAnimationFrame` 驅動遊戲循環
- **3 款純 DOM 操作**（點擊大師、金樸克、掃雷）
- **暗色太空主題** UI 設計系統，統一的 CSS 變數架構（`--bg-1`, `--accent`, `--danger` 等）
- **自製 AI** — 五子棋、黑白棋、中國象棋皆有實作 AI 對手
- **自製音效** — 部分遊戲使用 Web Audio API 合成音效，無外部音檔

---

## 快速開始

```bash
# 任何靜態檔伺服器均可
npx serve .
# 或
python3 -m http.server 8080
```

開啟瀏覽器訪問 `http://localhost:8080` 即可進入遊戲大廳。

---

## 專案結構

```
games/
├── README.md               # 本說明
├── index.html              # 遊戲大廳（入口）
├── 1.jpg                   # 預覽圖
├── snake.html              # 貪吃蛇
├── bee.html                # 小蜜蜂
├── tetris.html             # 俄羅斯方塊
├── breakout.html           # 打磚塊
├── memory.html             # 記憶翻牌
├── space.html              # 太空大戰
├── phoenix.html            # 火鳳凰
├── raiden.html             # 雷電飛機
├── blackjack.html          # 21 點
├── goldpoker.html          # 金樸克
├── gomoku.html             # 五子棋
├── bomberman.html          # 炸彈人
├── tank.html               # 坦克大戰
├── dinosaur.html           # 恐龍快跑
├── reversi.html            # 黑白棋
├── xiangqi.html            # 中國象棋
├── flappybird.html         # Flappy Bird
├── minesweeper.html        # 掃雷
├── clicker.html            # 點擊大師
└── streetfighter.html      # 快打旋風
```

---

## 遊戲大廳功能

`index.html` 提供完整的遊戲入口體驗：

- 🔍 **搜尋篩選** — 按名稱或關鍵字即時過濾遊戲
- 🎲 **隨機開玩** — 一鍵隨機進入遊戲
- 響應式設計 — 桌機與手機皆可瀏覽

---

## 授權

MIT License
