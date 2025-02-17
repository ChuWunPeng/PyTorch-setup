


## 目錄
1. [介紹](#介紹)
2. [安裝](#需安裝套件)
3. [GPU 相關安裝](#GPU)
4. [Conda](#conda)
5. [Git](#git)
----
## 介紹
目前2025， `tensorflow` 在易於產品開發的優勢， `PyTorch` 則是研究人員方便使用

初學者建議從 `Pytorch` 或 `tensorflow2 keras` 學習(API 套件)
ios and android 版 
TensorFlow.js => 把AI部署在網頁

----

## 需安裝套件
1. Anaconda3
2. Git
3. NVIDIA 驅動更新最高版本
4. CUDA Toolkit 對應驅動版本
5. cuDNN 對應CUDA版本
----
## 1. GPU
1. 下載[NVIDIA App](https://www.nvidia.com/zh-tw/software/nvidia-app/)

2. 驅動程式目錄下的工作室驅動程式，按更新
3. 下載 `CUDA Toolkit`，此為額外工具 ，這裡需注意 `NVIDIA CUDA` 版本為向下兼容，所以 Driver 12.8 可以安裝 CUDA Toolkit 12.6，而目前 PyTorch 也僅支援到12.6。
  ```bash
  nvcc -V
  ```
4. 下載 cuDNN 並把三個資料夾內的檔案（lib、）

----
## 2. Conda
```bash
conda create --n <環境名稱> python=3.9 #環境名稱建置
```
```bash
conda activate <環境名稱> #環境切換
```
```bash 
conda env list　#列出所有環境
```
```bash
conda install <套件名稱> #安裝套件
``` 
```bash
conda list #列出所有安裝套件
```
```bash
conda env export --name <環境名稱> > environment.yml #將環境資訊匯出至 YAML 檔
```
----

### 3. install PyTorch
至[PyTorch官網](https://pytorch.org/)，根據下載工具及自己的OS系統產生 Run this command，將其程式碼複製，並到 `conda` 產生的環境下安裝，最後cu 126的126為版本可自行修改成自己的版本
![image](https://github.com/user-attachments/assets/0d637fee-a2be-4613-9e85-7fd73fd5ee23)


## Git 版本控制
```bash
git config --global user.name "YourName" # 設定使用者名稱
git config --global user.email "YourEmail@example.com" #mail
```
```bash
git init #初始化 Git 儲存庫
```
```bash
git clone <遠端儲存庫URL> #複製（clone）遠端儲存庫
```
```bash
git status #檢視目前狀態
```
```bash
git add <檔案路徑> #將檔案加入暫存區
```
```bash
git add . # 全部加入暫存區
```
```bash
git commit -m "提交訊息" # 提交更改
```
```bash
git branch <分支名稱> # 建立分支
```
```bash
git checkout <分支名稱> # 切換分支
```
```bash
git push <遠端名稱> <分支名稱> #推送至遠端
```
```bash
git push origin main
```
```bash
git push -u origin main # 首次推送
```
```bash
git pull <遠端名稱> <分支名稱> # 取得遠端更新
```
----

