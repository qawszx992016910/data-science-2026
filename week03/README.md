# Week 03 打造地基：學習心得與任務檢核

### 🛠️ 1. WSL 與 Docker 環境解鎖心得
* **遇到的驚喜（Bug）：** 1. 在執行指令時，不小心在 Windows PowerShell 執行了 Linux 的 `supabase` 指令，導致系統報錯找不到程式。
    2. 在建立專案檔案時，漏掉了 `html` 資料夾就直接建立 `index.html`，結果出現 `No such file or directory`。
    3. 在 Docker 啟動前就執行 `status`，導致報錯說找不到容器（No such container）。
* **如何解決：** 1. 確認必須在 **WSL (Ubuntu)** 環境下操作。
    2. 使用 `mkdir -p html` 先建立路徑，再建立檔案。
    3. 確保 **Docker Desktop** 已啟動，並正確執行 `supabase start` 等待所有服務亮綠燈。

### ☁️ 2. Supabase 雲端專案初始化
* **Project URL:** https://abaqbyyeggqwnirieqyl.supabase.co
* **練習進度：** 已成功連結本地環境與雲端專案，並透過 Supabase Dashboard 建立資料表練習。

### 📂 3. JSON 資料建模練習
* 已建立 `config.json`，內容包含專案名稱、區域與啟用的功能清單，並確認格式符合標準。

### 🛡️ 4. Git 提交與資安習慣
* **.env**：已建立並加入 `.gitignore` 防止洩漏。
* **.env.example**：已建立空白範本供參考。

---

### ✅ Week 03 任務完成清單
- [x] WSL 2 環境運作正常
- [x] Docker 能成功啟動 `docker-compose.yml` 中的服務
- [x] Supabase 雲端專案已建立
- [x] 成功編輯 `config.json` 且格式正確
- [x] 已設定 `.gitignore` 保護敏感資訊
