# CLAUDE.md - 橋牌推廣教學參考資源專案指南

## 專案概述

本專案是一個**橋牌教學與推廣資源庫**,彙整了來自全球多個國際橋牌組織（ACBL、EBED、EBU、NZB、IBF、BAMSA 等）的教學材料、推廣文件和研究報告。專案以繁體中文為主要語言,提供中英對照的教學資源。

### 專案類型
- **靜態文檔網站**：純 HTML 文件展示型專案
- **知識庫**：橋牌教學資源彙整平台
- **教育資源**：適合教師、推廣者、學習者使用

### 主要特色
- 📚 豐富的國際橋牌教學資源
- 🌏 繁體中文翻譯與整理
- 📖 涵蓋推廣與教學兩大面向
- 🎯 從迷你橋牌（Mini-Bridge）到正式橋牌（Bridge）的完整教學路徑
- 🧠 包含運動心理學應用於橋牌競技的內容

---

## 專案結構

### 目錄架構

本專案採用**扁平化設計**,所有文件位於根目錄：

```
/home/user/bridge/
├── index.html                                           # 【主要入口】橋牌推廣教學參考資源索引
├── ArrowCards.png                                       # 唯一圖片資源
├── 在橋牌上取得心理優勢 Gaining the mental edge at bridge.md  # 唯一 Markdown 文件
│
├── 【推廣類文檔】
│   ├── 推庿心智運動橋牌的社會學研究搞要.html
│   ├── 推庿橋牌心智運動的社會學研究.html
│   ├── 橋牌：全民智力運動, BAMSA.html
│   ├── 為什麼要打橋牌.html
│   ├── 打橋牌的好處.html
│   ├── Why play_ from The Bridge World.html
│   ├── 人們為什麼打橋牌？.html
│   ├── ACBL Teacher Guidelines.html
│
├── 【教學類 - MiniBridge】
│   ├── EBED 迷你橋牌教學牌局.html
│   ├── ACBL 幼兒橋牌-教師手冊.html
│   ├── Elementary School Bridge Lesson Teacher Manual PreK-1st Grades.html
│   ├── EBU 迷你橋牌教師手冊.html
│   ├── NZB 第一課–簡介.html
│   ├── IBF Mini-Bridge.html
│   ├── EBED Minibridge Resources.html
│
└── 【教學類 - Bridge】
    ├── NZB 教師手冊.html
    └── The Bridge World Learning Center整理.html
```

### 文件分類說明

#### 1. 推廣類資源
主要用於橋牌推廣、說服學校或社區開設橋牌課程

| 組織 | 文件名稱 | 說明 |
|------|---------|------|
| BAMSA | 推廣心智運動橋牌的社會學研究 | 2024年社會學研究報告（含摘要與全文） |
| BAMSA | 橋牌：全民智力運動 | 2021年會議資料 |
| 綜合 | 為什麼要打橋牌 | 準備說帖用 |
| ACBL | Teacher Guidelines | 教師指南（與EBED類似,但需全盤照用） |

#### 2. 教學類資源 - MiniBridge（迷你橋牌）
適合初學者和兒童的簡化橋牌教學

| 組織 | 文件名稱 | 課程結構 |
|------|---------|----------|
| EBED | 迷你橋牌教學牌局 | 無王/王牌各10課,每課4牌;各加16牌複習;再加防禦各8牌 |
| ACBL | 幼兒橋牌-教師手冊 | 8課,6牌例（前四課介紹War, Tricks, Trumps, Whist） |
| EBU | 迷你橋牌教師手冊 | 12課,7頁習題,8練習牌例,術語表 |
| NZB | 第一課–橋牌簡介 | 迷你橋牌,4牌例 |
| IBF | Mini-Bridge | 17課,31牌例（加入開叫與答叫） |

#### 3. 教學類資源 - Bridge（正式橋牌）
進階橋牌教學材料

| 組織 | 文件名稱 | 課程結構 |
|------|---------|----------|
| IBF | From Mini-Bridge to Bridge | 18-41課,牌例32-83 |
| NZB | 教師手冊 | 10課（另有4課先教1NT開叫）,含學生筆記、測驗、牌例、教師筆記、PPT、影片、牌局檔案 |
| Bridge World | Learning Center整理 | 中文進行中 |

#### 4. 運動心理學資源
- `在橋牌上取得心理優勢 Gaining the mental edge at bridge.md`
- 內容包含：心理準備、積極心態、專注力、壓力管理、目標設定、比賽適應等

---

## 技術架構

### 技術棧

本專案採用**零建置工具**的純靜態網站架構：

#### 前端技術
- **HTML5**：所有頁面均為標準 HTML 文檔
- **CSS3**：內嵌樣式（來自 HackMD 導出）
  - Bootstrap 3.3.7
  - Font Awesome 4.7.0
  - Ionicons 2.0.1
  - Octicons 3.5.0
  - Prism 1.5.1（程式碼高亮）
- **JavaScript**：內嵌腳本
  - jQuery 3.1.1
  - Bootstrap JS
  - Gist Embed

#### 字型資源（Google Fonts）
- Roboto
- Source Code Pro
- Source Sans Pro
- Source Serif Pro

#### 內容格式
- **Markdown**：原始內容格式（已轉換為 HTML）
- **HackMD**：所有 HTML 文件都是從 HackMD 導出的靜態頁面

#### 版本控制
- **Git**：版本管理系統
- **GitHub**：遠端倉庫（`chrisokchen/bridge`）

### 重要特性

✅ **無需安裝依賴**：沒有 `package.json`、`requirements.txt` 等配置檔案
✅ **無需建置過程**：可直接在瀏覽器中打開 HTML 檔案
✅ **CDN 資源**：所有外部資源來自 CDN,無本地依賴
✅ **零配置**：無任何配置檔案
✅ **即開即用**：下載後立即可用

---

## 開發指南

### 本地開發

#### 方法一：直接開啟（推薦用於快速查看）
```bash
# 直接在瀏覽器中開啟任何 HTML 文件
open index.html  # macOS
xdg-open index.html  # Linux
start index.html  # Windows
```

#### 方法二：使用 HTTP 伺服器（推薦用於完整功能）
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Node.js (需先安裝 http-server: npm install -g http-server)
http-server -p 8000

# PHP
php -S localhost:8000
```

然後在瀏覽器中訪問 `http://localhost:8000`

### 內容編輯工作流程

#### 編輯 HTML 文件
1. 建議使用 **HackMD** 或其他 Markdown 編輯器編輯內容
2. 編輯完成後導出為 HTML
3. 將導出的 HTML 文件放入專案根目錄
4. 更新 `index.html` 中的連結（如有新文件）

#### 編輯 Markdown 文件
1. 直接編輯 `.md` 文件
2. 使用 Markdown 預覽工具檢查格式
3. 提交變更

#### 更新索引頁面
1. 開啟 `index.html`
2. 在適當的表格中新增或更新連結
3. 保持表格結構一致：組織 | 英文 | 中文 | 說明

### Git 工作流程

```bash
# 查看當前狀態
git status

# 新增變更
git add <文件名>

# 提交變更
git commit -m "描述變更內容"

# 推送到遠端
git push -u origin <分支名>
```

---

## 部署方式

本專案可輕鬆部署到多種靜態網站託管服務：

### GitHub Pages（推薦）
1. 在 GitHub 倉庫設置中啟用 GitHub Pages
2. 選擇主分支作為來源
3. 網站將自動部署到 `https://<username>.github.io/<repository>`

### Netlify
1. 連接 GitHub 倉庫
2. 無需配置建置命令
3. 自動部署

### Vercel
1. 連接 GitHub 倉庫
2. 無需配置
3. 自動部署

### 自建伺服器
使用任何 HTTP 伺服器（Nginx、Apache 等）直接提供靜態文件服務。

---

## AI 助手應遵循的主要慣例

### 1. 語言使用規範

**絕對規則**：
- ✅ **一律使用繁體中文**撰寫所有文檔內容
- ✅ 保留專業術語的英文原文（如：MiniBridge、ACBL）
- ✅ 組織名稱使用英文縮寫
- ✅ 技術術語可中英並列（首次出現時）

**範例**：
```markdown
✅ 正確：EBED（English Bridge Education & Development）提供的迷你橋牌（MiniBridge）教學資源
❌ 錯誤：EBED 提供的 mini bridge teaching resources
```

### 2. 文件命名規範

**HTML 文件**：
- ✅ 使用繁體中文命名（如：`為什麼要打橋牌.html`）
- ✅ 可使用中英混合（如：`ACBL Teacher Guidelines.html`）
- ✅ 保持與原始來源一致的命名風格

**Markdown 文件**：
- ✅ 使用描述性中文名稱
- ✅ 可附加英文原文（如：`在橋牌上取得心理優勢 Gaining the mental edge at bridge.md`）

### 3. 內容組織規範

**結構原則**：
- 📁 維持扁平化目錄結構（所有文件在根目錄）
- 📑 `index.html` 作為唯一入口點
- 🔗 所有文件必須在 `index.html` 中有對應連結
- 📊 使用表格組織資源（推廣 / 教學 - MiniBridge / 教學 - Bridge）

**分類標準**：
```
推廣類 → 用於說服、宣傳、研究報告
教學類 - MiniBridge → 適合初學者、兒童
教學類 - Bridge → 進階學習者
運動心理學 → 競技相關心理技巧
```

### 4. 編輯文件時的注意事項

**編輯 HTML 文件**：
- ⚠️ 保留所有 HackMD 導出的樣式和腳本
- ⚠️ 不要移除 CDN 連結
- ⚠️ 保持 Bootstrap 表格結構完整
- ⚠️ 確保所有連結使用相對路徑

**編輯 Markdown 文件**：
- ✅ 使用標準 Markdown 語法
- ✅ 保持清晰的標題層級
- ✅ 使用列表和表格增強可讀性
- ✅ 適當使用引用和程式碼區塊

### 5. 新增內容時的流程

當需要新增教學資源時：

```markdown
1. 確定資源類型（推廣/MiniBridge/Bridge）
2. 建立或轉換 HTML 文件（使用 HackMD）
3. 使用繁體中文命名文件
4. 將文件放置在根目錄
5. 更新 index.html 中對應的表格
6. 確保表格包含：組織 | 英文 | 中文 | 說明
7. 提交變更到 Git
```

**表格更新範例**：
```html
<tr>
  <td><a href="https://www.acbl.org/" target="_blank">ACBL</a></td>
  <td><a href="原始英文連結" target="_blank">英文標題</a></td>
  <td><a href="本地中文檔案.html" target="_blank">中文標題</a></td>
  <td>說明文字</td>
</tr>
```

### 6. 文檔風格指南

**標題規範**：
```markdown
# H1 - 主標題（每頁一個）
## H2 - 章節標題
### H3 - 小節標題
#### H4 - 子小節（謹慎使用）
```

**列表使用**：
- 使用無序列表 (`-` 或 `*`) 表示並列項目
- 使用有序列表 (`1.`, `2.`) 表示步驟或順序
- 使用任務列表 (`- [ ]` / `- [x]`) 表示待辦事項

**強調和格式**：
- **粗體**：重要概念、關鍵詞
- *斜體*：外文術語、引用
- `程式碼`：指令、檔案名稱、程式碼片段
- > 引用：引述他人觀點、重要說明

### 7. 連結處理規範

**內部連結**：
```html
<!-- 使用相對路徑 -->
<a href="為什麼要打橋牌.html">為什麼要打橋牌</a>
```

**外部連結**：
```html
<!-- 使用 target="_blank" 和 rel="noopener" -->
<a href="https://www.acbl.org/" target="_blank" rel="noopener">ACBL</a>
```

### 8. 圖片資源處理

**目前狀態**：
- 專案中僅有一個圖片：`ArrowCards.png`
- 所有其他資源來自 CDN

**新增圖片時**：
```markdown
1. 圖片放置在根目錄（維持扁平結構）
2. 使用描述性中文命名（如：橋牌教學示意圖.png）
3. 在 HTML 中使用相對路徑引用
4. 考慮圖片大小（建議 < 500KB）
```

### 9. 版本控制規範

**Commit 訊息格式**（使用繁體中文）：
```
新增：新增 XXX 教學資源
更新：更新 XXX 文件內容
修正：修正 XXX 錯誤
移除：移除過時的 XXX 文件
整理：重新整理 XXX 結構
```

**分支命名**：
```
claude/create-claude-md-011zcYssjwWokHuxjXsaTpnw  # 當前功能分支
```

### 10. 資料來源標註

**每個資源必須標註**：
- 📌 來源組織（ACBL / EBED / EBU / NZB / IBF / BAMSA）
- 🔗 原始連結（如有）
- 📅 發布/更新日期（如有）
- 📝 翻譯或整理者（如適用）

**範例**：
```html
<tr>
  <td><a href="https://www.ebedcio.org.uk/">EBED</a></td>
  <td><a href="原始PDF連結">MiniBridge Teaching Hands</a></td>
  <td><a href="EBED 迷你橋牌教學牌局.html">EBED 迷你橋牌教學牌局要點</a></td>
  <td>分無王/王牌各10課，每課4牌；各加16牌複習;再加防禦各8牌</td>
</tr>
```

---

## 常見問題 (FAQ)

### Q1: 為什麼所有文件都在根目錄？
A: 本專案採用扁平化設計,簡化結構,方便直接開啟和管理。這是有意的設計選擇。

### Q2: 可以新增子目錄嗎？
A: 不建議。請維持現有的扁平結構,保持專案一致性。

### Q3: 如何新增新的教學資源？
A:
1. 使用 HackMD 編輯內容
2. 導出為 HTML
3. 使用繁體中文命名
4. 放入根目錄
5. 更新 `index.html`
6. 提交到 Git

### Q4: 是否需要建置工具？
A: **完全不需要**。本專案零建置,零配置,即開即用。

### Q5: 如何處理多語言內容？
A:
- 主要語言：繁體中文
- 保留英文原文連結和組織名稱
- 技術術語可中英並列

### Q6: 圖片和媒體檔案如何處理？
A:
- 放在根目錄
- 使用描述性中文命名
- 控制檔案大小
- 考慮使用 CDN（大型媒體）

---

## 資源連結

### 國際橋牌組織
- [ACBL (American Contract Bridge League)](https://www.acbl.org/)
- [EBED (English Bridge Education & Development)](https://www.ebedcio.org.uk/)
- [EBU (English Bridge Union)](https://www.ebu.co.uk)
- [NZB (New Zealand Bridge)](https://www.nzbridge.co.nz/)
- [IBF (Israel Bridge Federation)](https://main.bridge.co.il/)
- [BAMSA (Bridge: A MindSport for All)](https://bridgemindsport.org)
- [Bridge World](https://www.bridgeworld.com)

### 相關資源
- [2024教練橋藝運動心理學資源目錄](https://drive.google.com/drive/folders/1LJilYhqqWe5GumMgM3qgEg2B9Ooup89Q)

---

## 維護者資訊

本專案由 **chrisokchen** 維護。

如需協助或有任何問題,請透過 GitHub Issues 聯繫。

---

## 授權聲明

本專案彙整的資源來自多個國際橋牌組織,版權歸原作者所有。

繁體中文翻譯和整理部分由專案貢獻者提供。

---

## 更新日誌

### 2025-11-17
- ✅ 建立 CLAUDE.md 文件
- ✅ 完整記錄專案結構和開發規範
- ✅ 建立 AI 助手協作指南

---

**最後更新**：2025-11-17
**文件版本**：1.0.0
**維護者**：chrisokchen
**專案狀態**：活躍維護中 🟢
