title: git 基礎
author: ian
date: 2024-01-23 15:56:52
tags:
---
## 初次運行配置


#### 建議安裝套件
> git graph
![upload successful](\blog.github.io\images\pasted-0.png)

#### 用戶信息設置
```
git config --global user.name "ian"
git config --global user.email ian@example.com
```

<font color="red">查看配置</font>
```
git config --list
```

#### 初次使用
```
git init
git add .
git commit -m "註釋"  
git remote add origin https://github.com/ianiani910425/example.git
git push -u origin main
```
<font color="red"> commit 一定要註釋，且此時的commit並未上傳，只暫存在本地倉庫 </font></br>
<font color="green"> 本地倉庫名預設為origin </font></br>


#### 複製倉庫到本地
```
git clone [url]
```
#### 同步目前網上內容
```
git pull origin main
```
#### 分支
###### 創建分支
```
git branch [name]
```
###### 查看分支
```
git branch -v
```
###### 分支改名
```
git branch -v [branch_name] [new_branch_name]
```
###### 刪除分支
```
git branch -d [branch_name]
```
###### 切換分支
```
git checkout [branch_name]
```
###### 分支合併:
先確認目前所在分支，再merge其他分支
```
git merge [另一個預合併分支]
```

#### 撤銷
先查看git紀錄
```
git log --oneline
```
再刪除
```
git reset [填入剛才的id 或 名字 或 HEAD]
```