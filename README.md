## 說明文件

1. `chmod +x get_data.sh` (賦予該執行檔執行權限)
2. `./get_data.sh` (產生ECG-data中的ICBEB/PTBXL兩個dataset, 並解壓縮模型)
該執行檔會產生兩組dataset及Production，Production中會有
3. `pip3 install -r requirements.txt` (安裝環境套件)
4. `cd Code-final`
5. `python3 SPN_Online_Infernece.py ICBEB`
6. `python3 SPN_Online_Infernece.py PTBXL`

```
dirTree  －－－－－－根目录
  │
  ├─lib  －－－－－－相关函数目录
  │  │
  │  └─dirTree.js  －－－－－－相关函数接口
  │
  ├─README.md  －－－－－－说明文档
  │
  ├─conf.js  －－－－－－配置文件
  │
  └─tree.js  －－－－－－入口文件
```
