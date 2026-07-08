# 銀河遊戲大廳 · Galaxy Game Arcade

<p align="center">
  <img src="assets/images/logo.png" alt="銀河遊戲大廳 Logo" width="220">
</p>

一個純前端的經典遊戲合集。所有遊戲都以單檔 HTML 製作，入口大廳提供搜尋、分類篩選與隨機開玩，開啟靜態伺服器就能直接遊玩。

## 線上展示

GitHub Pages: https://jimmywon1028.github.io/games/

---

## 目前內容

- **21 款遊戲**，涵蓋街機、射擊、益智、棋類、卡牌與動作類型
- **無框架、無打包流程**，主要使用 HTML / CSS / JavaScript / Canvas 2D
- **遊戲大廳**支援關鍵字搜尋、分類篩選、顯示數量與隨機進入遊戲
- **迷魂車**使用 `assets/audio/` 內的專屬 MP3 音效與 BGM
- 圖片與音效資產已集中到 `assets/`，遊戲頁集中到 `games/`

---

## 遊戲列表

| 遊戲 | 分類 | 檔案 | 玩法重點 |
|---|---|---|---|
| 貪吃蛇 | 街機 / 休閒 | `games/snake.html` | 控制蛇吃食物、避免撞牆與撞到自己 |
| 小蜜蜂 | 射擊 | `games/bee.html` | 縱向射擊、閃避敵機並推進關卡 |
| 俄羅斯方塊 豪華版 | 益智 / 消除 | `games/tetris.html` | 方塊消除、暫存區與下一顆預覽 |
| 打磚塊 | 街機 | `games/breakout.html` | 控制板子反彈球，擊碎所有磚塊 |
| 記憶翻牌 | 益智 | `games/memory.html` | 翻牌配對，考驗記憶力 |
| 太空大戰 | 射擊 | `games/space.html` | 橫向太空射擊，閃避敵機 |
| 火鳳凰 | 射擊 | `games/phoenix.html` | 鳳凰主題飛行射擊 |
| 雷電飛機 | 射擊 | `games/raiden.html` | 縱向彈幕射擊 |
| 21 點 | 卡牌 | `games/blackjack.html` | Blackjack 規則，和莊家比點數 |
| 金樸克 | 卡牌 | `games/goldpoker.html` | 街機 Video Poker 玩法 |
| 五子棋 | 棋類 | `games/gomoku.html` | 人機對弈，先連五子獲勝 |
| 炸彈人 | 動作 | `games/bomberman.html` | 迷宮放炸彈、爆破障礙與敵人 |
| 迷魂車 豪華版 | 街機 / 迷宮 | `games/rallyx.html` | Rally-X 風格追逐、雷達、旗子、煙霧與專屬音效 |
| 坦克大戰 | 動作 | `games/tank.html` | Battle City 風格坦克對戰 |
| 恐龍快跑 | 街機 / 跑酷 | `games/dinosaur.html` | 跳躍閃避障礙 |
| 黑白棋 | 棋類 | `games/reversi.html` | 翻轉棋子、爭取最大盤面 |
| 中國象棋 | 棋類 | `games/xiangqi.html` | 中國象棋人機對弈 |
| Flappy Bird | 街機 | `games/flappybird.html` | 點擊飛越管道 |
| 掃雷 | 益智 | `games/minesweeper.html` | 推理格子，避開地雷 |
| 點擊大師 | 街機 / 放置 | `games/clicker.html` | 點擊升級與放置成長 |
| 快打旋風 | 動作 / 格鬥 | `games/streetfighter.html` | 1v1 格鬥對戰 |

---

## 快速開始

這是純靜態專案，使用任何靜態檔伺服器都可以。

```bash
python3 -m http.server 8080
```

開啟：

```text
http://localhost:8080
```

也可以使用其他靜態伺服器，例如：

```bash
npx serve .
```

---

## 專案結構

```text
games/
├── index.html              # 遊戲大廳入口
├── README.md               # 專案說明
├── AGENTS.md               # Codex 維護規則
├── assets/
│   ├── images/
│   │   └── logo.png        # 專案 Logo
│   └── audio/
│       ├── 01_High Score.mp3
│       ├── 02_Level BGM.mp3
│       ├── 03_Level Finish.mp3
│       ├── 04_Bonus Round Start.mp3
│       └── 05_Game Start.mp3
└── games/
    ├── snake.html
    ├── bee.html
    ├── tetris.html
    ├── breakout.html
    ├── memory.html
    ├── space.html
    ├── phoenix.html
    ├── raiden.html
    ├── blackjack.html
    ├── goldpoker.html
    ├── gomoku.html
    ├── bomberman.html
    ├── rallyx.html
    ├── tank.html
    ├── dinosaur.html
    ├── reversi.html
    ├── xiangqi.html
    ├── flappybird.html
    ├── minesweeper.html
    ├── clicker.html
    └── streetfighter.html
```

---

## 維護重點

- 新增遊戲時，同步更新 `index.html` 的卡片與本 README 的遊戲列表。
- 遊戲頁放在 `games/`，圖片放在 `assets/images/`，音效放在 `assets/audio/`。
- 檔名含空白的音效在 HTML 中要使用 URL encoded 路徑，例如 `%20`。
- 單一遊戲修改後，至少確認頁面可載入、console 無明顯錯誤、鍵盤或觸控主要操作可用。

---

## 授權

MIT License
