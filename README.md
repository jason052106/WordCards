# WordCards 單字卡程式

## 📖 專案簡介 (Introduction)
WordCards 是一個使用 C# Windows Forms 開發的單字學習應用程式。本專案提供直覺的操作介面、單字發音功能，以及方便的自動播放與快捷鍵設計，讓使用者能有效率地進行單字背誦與學習。

## ✨ 核心功能 (Features)
* **資料檔讀取：** 程式啟動時會自動讀取 TSV 格式的單字檔 (`WordCards.txt`)，載入單字、音標、音檔路徑與解釋。
* **單字顯示與發音：** 點選單字清單，即可顯示詳細內容並透過內建的 `Windows Media Player` 元件播放對應的 MP3 發音。
* **自動播放模式：** 支援設定時間間隔（Interval）的自動輪播功能，方便使用者連續聆聽與學習 。
* **快捷鍵操作：**
    * 按下 `Enter` 鍵：切換至下一個單字並播放發音 。
    * 按下 `Space` (空白鍵)：重複播放目前單字的發音。
* **單字即時編輯與儲存：** 雙擊單字清單，可開啟編輯視窗修改單字內容，儲存後會即時更新並寫回文字檔 。

## 🛠️ 開發環境與技術 (Environment & Technology)
* **開發語言：** C#
* **開發框架：** .NET Framework 4.8 (Windows Forms) 
* **外部參考元件：** `Windows Media Player` (WMPLib) 用於音效播放 。
* **自訂集合類別：** 實作 `WordItem` 類別封裝單字屬性，並繼承 `Collection<WordItem>` 建立自訂的 `WordCollection` 集合，提升資料管理的效率。

## 📂 資料檔格式說明 (Data Format)
系統預設讀取專案目錄下的 `WordCards.txt`，請確保該檔案編碼為 **Unicode**，以正常顯示音標。

## 如何執行
確認你的電腦已安裝 Visual Studio，並包含 .NET 桌面開發 工作負載。

將本專案下載或 Clone 到本機。

在專案資料夾中找到 .sln (方案檔) 並雙擊開啟。

按下鍵盤的 F5 或是點擊上方的「開始」按鈕，即可編譯並執行程式。

## 執行畫面
<img width="724" height="432" alt="螢幕擷取畫面 2026-06-03 155037" src="https://github.com/user-attachments/assets/5a36d934-1898-4a6f-b3e4-fb46b86ee593" />

