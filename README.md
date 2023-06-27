# screenshot_QRcode_reader

### 利用opencv中的qrcode reader辨識所框選的QRcode

### used package:

  `tkinter`, `PIL`, `cv2`
  
我有利用 `pyinstaller`包裝成 `.exe`，但由於 `opencv`套件過於龐大，超過github上傳檔案大小限制，所以無法上傳。
後續會跟大家說明如何自行包裝成`.exe`
## 使用方法
### 一、直接執行[screenshot.py](./screenshot.py)
1. 確認函式庫是否包含上述三個非內建函式庫。
2. 確認後直接執行[screenshot.py](./screenshot.py)

### 二、包裝成 `.exe`格式

1. 確認函式庫中是否有pyintsaller，如果無的話可以在終端機中執行下列命令: 
   ```
   pip install pyinstaller
   ```
2. 確認安裝pyintsaller後，cd到clone的資料夾中。
3. 執行下列命令:
   ```
   pyinstaller -F -w --hidden-import "opencv-python"  "screenshot.py"
   ```
4. clone資料夾中會出現 `dist` 跟 `build`資料夾， `.exe`檔案就在`dist`資料夾中。
   
