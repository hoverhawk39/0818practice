# 三個 Gemini 練習小工具 (0818practice)

本專案收錄由 Gemini 輔助開發的三個獨立 Web 實用小工具，並提供現代化響應式（RWD）首頁 [`index.html`](index.html) 進行整合導覽與即時預覽。

🔗 **線上正式版網址**：[https://gemini-0818practice.netlify.app](https://gemini-0818practice.netlify.app)

---

## 🌟 專案首頁

- **首頁檔案**：[`index.html`](index.html)
- **線上網址**：[https://gemini-0818practice.netlify.app](https://gemini-0818practice.netlify.app)
- **特色**：
  - 現代深色科技美學（Luminous Dark Glassmorphism）
  - RWD 全響應式設計（手機 / 平板 / 桌面）
  - 類別標籤即時篩選（財務分析、個資安全、待辦同步）
  - 內建彈出式即時預覽視窗（Modal Preview）與新分頁快速開啟

---

## 🛠️ 收錄小工具一覽

### 1. 📈 台股合併現金流量表財務分析 Dashboard ([`dashboard.html`](dashboard.html))
- **技術棧**：HTML5, Tailwind CSS, SheetJS (xlsx), ECharts, FontAwesome
- **核心功能**：
  - 本地端 Excel 財報拖曳解析（100% 離線運算）
  - 內建台積電（2330）標準格式示範數據一鍵載入
  - 營業現金流 (OCF)、資本支出 (CapEx)、自由現金流 (FCF) 指標分析
  - 動態現金流轉化瀑布圖與科目增減比較表格

### 2. 🛡️ 本地端個資假名化與脫敏工具 ([`local_anonymizer_tool.html`](local_anonymizer_tool.html))
- **技術棧**：HTML5, Tailwind CSS, SheetJS, CryptoJS, FontAwesome
- **核心功能**：
  - 4 步驟流水線作業：上傳 ➔ 規則設定 ➔ 預覽脫敏 ➔ 匯出
  - 支援多種遮蔽策略：字元遮罩、加鹽雜湊 (Salted SHA-256)、數值位移、日期位移
  - 產生並匯出獨立保密金鑰對照表（Key Mapping）
  - 純本機瀏覽器運算，資料絕不上傳雲端

### 3. ⚡ TaskPulse - 跨裝置同步待辦事項 ([`taskpulse_sync_todo.html`](taskpulse_sync_todo.html))
- **技術棧**：HTML5, Tailwind CSS, Firebase / Firestore, LocalStorage Fallback, FontAwesome
- **核心功能**：
  - 通行碼（Passcode）多房間即時同步機制
  - 支援無網路/離線模式，自動降級至瀏覽器 LocalStorage 持久化儲存
  - 任務分類（工作/個人/學習/財務/健康）、優先級標籤與到期日警示
  - 多層級子任務清單與動態完成率統計

---

## 🚀 快速啟動

直接使用任何現代瀏覽器開啟 `index.html` 即可：

```bash
open index.html
```

或使用 Python 簡易本機伺服器：

```bash
python3 -m http.server 8000
# 接著於瀏覽器開啟 http://localhost:8000
```
