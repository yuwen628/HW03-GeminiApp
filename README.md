
Demo Website: https://yuwen628.github.io/HW03-GeminiApp/

# WH3-WebApp — AI 畫布生成器

支援 **Google Imagen 4.0**（Gemini API）與 **NVIDIA Cosmos 3**（Hugging Face Inference API）的多模型圖像生成平台。

## 功能特色

- **雙模型切換** — 無縫切換 Imagen 4.0 與 Cosmos 3，每個模型提供專屬控制項（負向提示詞、推理步數、CFG 引導係數、畫面比例）
- **Gemini 智能優化** — 透過 `gemini-2.5-flash-preview` 將簡短點子擴寫成高品質提示詞
- **連線診斷工具** — 一鍵測試 API 連線狀態，附 DNS/網路排除建議
- **本地歷史紀錄** — 自動儲存生成記錄，支援重播與管理（`localStorage` 持久化）
- **深色主題 UI** — 現代化暗色介面搭配黃色主題，採用 Tailwind CSS 與 Lucide 圖標

## 快速開始

無需建置，直接用瀏覽器開啟 `index.html` 即可使用。

### API 金鑰

- **Imagen 4.0**：需在運行環境中注入 Gemini API 金鑰
- **Cosmos 3**：在介面中輸入 Hugging Face User Access Token（本地儲存）

## 技術棧

- 原生 JavaScript（無框架）
- Tailwind CSS（CDN）
- Lucide Icons（CDN）
- Hugging Face Inference API
- Google Gemini API（Imagen 4.0 + 提示詞優化）

## 使用方式

1. 從下拉選單選擇生成模型
2. 輸入提示詞（或使用 Gemini 優化 / 靈感庫）
3. 調整進階參數（Cosmos 3：負向提示詞、步數、CFG、比例）
4. 點擊「開始生成圖像」等待結果
