# Ruffle 0.7.1（自架播放器）

來源：官方發行檔 https://github.com/ruffle-rs/ruffle/releases/download/v0.7.1/ruffle-0.7.1-web-selfhosted.zip

此處保留發行檔的 ruffle.js、兩個 core JavaScript、兩個 WebAssembly、package.json 與 Apache/MIT 授權文件，未修改第三方程式。不使用 CDN；播放器由本站提供，只有按下「啟動虛擬導覽」後才下載。升級時應整組替換同版檔案，再驗證桌面與手機觸控。

原站素材另置於 `/virtual-tour/3d.swf`，原始來源 `legacy-site/02/3d.swf`，大小 32,799,518 bytes；SHA-256 為 `ad6ba58856e269b5270bc2b7248f9f8c8d0e10b3d5a0b8377ea57ca6a476b9e0`。原檔未修改，不屬於 Ruffle 授權素材。

SWF 內含場景照片與操作箭頭，不需外部場景 API。停用 Flash 對頁面 JavaScript 的存取及開啟外部連結；不將播放器設定視為完整網路隔離機制。載入原檔有 60 秒逾時，停止時移除播放器、釋放場景。

已使用 Chromium 與 WebKit 的桌面及手機觸控模擬確認前進、左右轉、4:3 自適應顯示、停止重開與失敗重試。WebKit 測試不等同真實 Safari；尚未完成真實 iPhone／Android 與 Safari 相容性驗證。原始檔與引擎體積較大，行動網路首次啟動可能較慢。關閉硬體加速的瀏覽器可能顯示 Ruffle 效能警告；不隱藏此警告。
