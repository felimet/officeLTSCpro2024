# 透過官方下載，永久免費使用正版 Office !

## 1. 配置文件 (config.xml) 包含
- **Office LTSC Professional Plus 2024**
- **Visio LTSC Professional 2024**
- **Project Professional 2024**

---

## 2. 參考資源

### 參考教學影片
[觀看教學影片](https://youtu.be/vRCV38wrl9s?si=r_Bh9LgAOzSRO-0J) 
- REF：零度解说. (2024, October 16). *永久免费使用正版Office!微软官方 LTSC 2024 长期服务版安装教程 ,简单易懂!| 零度解说* [Online]. YouTube. https://www.youtube.com/watch?v=vRCV38wrl9s

### 下載與工具
1. **Office 軟體部署工具**：  
   [下載連結](https://www.microsoft.com/en-us/download/details.aspx?id=49117)

2. **Office 版本自訂工具**：  
   [開啟工具](https://config.office.com/deploymentsettings)

3. **基於 KMS 的 GVLK**：  
   [官方文檔](https://learn.microsoft.com/zh-cn/deployoffice/vlactivation/gvlks)

---

## 3. 安裝步驟

### **❗ 先移除舊版本**

1. **進入 `office_2024_x64` 資料夾**
2. **以管理員身份執行 CMD 進入命令終端**
3. **在 CMD 中無法轉跳到其他資料夾解決方法，使用 `cd /d yourPath`**

### **步驟 1：下載 Office 安裝檔案 (該儲存庫中已有 config.xml，可略。)**
```sh
setup /download config.xml
```

### **步驟 2：安裝 Office**
```sh
setup /configure config.xml
```

### **步驟 3：啟動 Office**
```sh
cd C:\Program Files\Microsoft Office\Office16
```
```sh
cscript ospp.vbs /sethst:kms.03k.org
```
```sh
cscript ospp.vbs /act
```

---

## 4. 注意事項
- ❗確保 `config.xml` 配置正確。
- ❗使用管理員身份執行命令，避免權限問題。
- ❗若無法正常啟動產品，再重新執行「步驟 3」。
- 若安裝過程中遇到錯誤，可參考 [Microsoft 官方指南](https://learn.microsoft.com/) 進行排除。

---

## 5. **額外說明**
- 該 `config.xml` 為 Office LTSC 2024 版本。
- 若需安裝其他版本與軟體，請參考 [2. 參考資源](#2-參考資源)。


