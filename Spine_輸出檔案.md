# Spine 輸出檔案


## 選單功能

![](img/2023-03-01%2022_41_51.png)
![](img/2023-03-01%2023_03_00.png)

檔案相關
+ `New Project` - 新增專案
+ `Open Project` - 開啟專案
+ `Recent Projects` - 最近專案
+ `Save Project` - 儲存專案
+ `Save Project As` - 專案另存為

編輯相關
+ `New Skeleton` - 新增骨架

輸出相關  
+ `Import Project` - 匯入專案，`.Spine` 檔案重新載入，不同版本不相容
+ `Import Data` - 匯入資料，`.Json` `.Binary` 檔案重新載入
+ `Export` - 匯出，輸出成 `.Json` `.Binary` 圖片或影片
+ `Texture Packer` - 材質打包器，輸出成 `.atlas` 與合併的 `.png`
+ `Texture Unpacker` - 材質解包器，`.atlas` 載入重新把合併的 `.png` 拆分獨立
  
平台設定
+ `Settings` - 設定，設置語言，熱鍵...等

## 重新載入

1. `.Spine` 檔案，使用 `Import Project` or `Open Project`，不同版本不相容，不推薦
2. `.Json` `.Binary` `.atlas`檔案，使用 `Import Data`，沒有圖檔則不會載入圖片
3. `.atlas` `.png` 檔案，使用 `Texture Unpacker`，資料夾設置為預設名稱 `.\images`


## 參考

http://zh.esotericsoftware.com/spine-texture-packer