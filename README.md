## 說明文件

1. `chmod +x get_data.sh` (賦予該執行檔執行權限)
2. `./get_data.sh` (產生ECG-data中的ICBEB/PTBXL兩個dataset, 並解壓縮模型)

```
Production  - - - - - -模型目錄
  │
  ├─CNNLSTM  - - - - - -SPN-V2 backbone模型
  │  │─ICBEB─1─pretrained.pt
  │  └─PTBXL  - 1 - pretrained.pt
  │
  ├─models  －－－－－－最終模型
  │  |─KGEVO
  |  |  |─ICBEB  －－－－－－ Dataset1 KGEVO 最終模型
  |  |  └─PTBXL  －－－－－－ Dataset2 KGEVO 最終模型
  |  └─SPN_V1
  |  |  |─ICBEB  －－－－－－ Dataset1 SPN 最終模型
  |  |  └─PTBXL  －－－－－－ Dataset2 SPN 最終模型
  │
  ├─state  －－－－－－配置文件
  │
  └─weights  －－－－－－入口文件
```

3. `pip3 install -r requirements.txt` (安裝環境套件)
4. `cd Code-final`
5. `python3 SPN_Online_Infernece.py ICBEB`
6. `python3 SPN_Online_Infernece.py PTBXL`

