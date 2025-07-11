# 永續綠色金融—資料前處裡
### 主旨
為了建立中信永續智慧問答系統，首先收集中信永續相關資料（PDF檔），接著使用 Unstructured 解析 PDF 檔內容，將 PDF 檔內容轉成 Json 檔。

### 方法流程
1. 在 VM(Oracle VirtualBox) 中安裝 Ubuntu 22.01.5 LTS 系統
2. 在 Ubuntu 中安裝 Docker
3. 在 Docker 中部屬 unstructured image 檔
4. Run 一個 Container 使用 unstructured image 服務
5. VsCode 連線到剛 run 的 Container
6. 使用 Jupyter 執行 python 城市檔

### 目前狀況（20250711）
解析出的 Json 檔內容，Type 標籤對的不准。

例如：原本是文本內容，但 Type 被標記成 Title。

Type 種類分成：Title、NarrativeText、UncategorizedText、Footer、ListItem。
