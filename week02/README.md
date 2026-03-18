# Week 02：資料集分析作業

本作業針對 **TFT (Teamfight Tactics, 雲頂之弈)** 相關主題，從 Kaggle 與 Google Dataset Search 挑選兩個資料集進行分析。

## 資料集對照表

| 項目 | 資料集 1 | 資料集 2 |
| :--- | :--- | :--- |
| **資料集名稱** | [TFT Match Data (Set 3 & 4)](https://www.kaggle.com/datasets/gyejr95/tft-match-data) | [TFT Global Master+ Rank Data](https://datasetsearch.research.google.com/search?src=0&query=TFT&docid=L2cvMTFsbGI5ZHBzNg%3D%3D) |
| **來源平台** | Kaggle Datasets | Google Dataset Search |
| **資料格式** | CSV | JSON / CSV |
| **資料筆數** | 約 10,000+ 場比賽紀錄 | 約 50,000+ 位高階玩家數據 |
| **主要欄位** | 1. `gameId` (比賽編號)<br>2. `placement` (最終名次)<br>3. `combination` (陣容羈絆)<br>4. `unit` (登場英雄單位)<br>5. `last_round` (結束回合) | 1. `summonerName` (玩家名稱)<br>2. `tier` (階級段位)<br>3. `leaguePoints` (勝點分數)<br>4. `wins` (勝場數)<br>5. `losses` (敗場數) |
| **可解決的問題** | 1. 分析特定版本最強的陣容搭配 (Meta)。<br>2. 計算特定英雄或裝備對前四名勝率的影響力。 | 1. 分析全球高階玩家的排位分數分佈。<br>2. 研究特定玩家在長期對戰中的勝率穩定度。 |
| **資料品質評估** | **優點：** 欄位精細度極高，適合做細部的戰術分析。<br>**缺點：** 屬於舊賽季數據，對於當前版本的即時參考價值較低。 | **優點：** 數據樣本龐大且涵蓋全球，具備高度統計代表性。<br>**缺點：** 原始 JSON 格式包含多層巢狀結構，初步清理數據較繁瑣。 |

---
**作業維護者：** B11356022
