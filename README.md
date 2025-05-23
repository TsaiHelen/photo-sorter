# Photo Sorter 相片分檢系統

## 專案目標
這是一個用來整理與分類大量相片檔案的工具。主要目的是協助使用者，從一大堆檔案中快速篩選出符合特定條件的照片，方便後續整理、備份或管理。

目前設計為二階段流程：
1. 分檢後，純文字輸出符合條件的清單 (不動原檔)
2. 提供選項，將符合條件的相片 copy 或 move 到指定目錄

---

## 核心功能 (持續開發中)
|功能|說明|
|----|----|
|依檔案大小分類|大於或小於指定 MB 或 KB|
|依解析度分類|Ex: 低解析度、4K、8K|
|判斷有人臉|利用人臉偵測模組|
|判斷是否為截圖|判斷 EXIF 或手機截圖特徵|
|純文字輸出|列出符合條件的檔案清單|
|搬移或複製|選擇性執行|

---

## 技術規劃
- 開發語言：Python
- 架構設計：模組化
- 第三方模組：
  - Pillow (影像處理)
  - exifread / piexif (讀取EXIF)
  - OpenCV / face_recognition (人臉偵測)
  - 其他開源好用的模組會視需要引用

---

## 專案理念
> 自行開發為主，開放整合現有優秀的開源工具，目標是打造一個「簡單、實用、容易擴充」的相片分檢系統。

---

## License
MIT License  
自由使用，請保留原作者資訊。

---

## TODO
- [ ] 初版 CLI 介面
- [ ] 檔案搜尋與條件篩選模組
- [ ] 輸出結果檔案
- [ ] Copy / Move 功能
- [ ] 增加人臉偵測功能
- [ ] 增加手機截圖判斷功能

