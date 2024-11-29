### git優點
速度小、檔案小
同時支援本地及遠端操作 (不需要網路)

```py
# 檢視目前設定
git config --list

# 設定username 及 email
git config --global user.name "elaine"
git config --global user.email "lioou.work@gmail.com"
```

要去為你自己學git 上面找 終端機常見指令

### git 執行流程
工作目錄 Working
暫存區域 Staging
儲存庫 Repository

staging area
commit -m "init commit" 
git help
git status

### git Command 指令
git init    初始化 
git status
git commit -m "init commit" 
git add .. (..代表上層)
git add .  (.代表這裡/這一層) 
git add --all  
git checkout .   把檔案或目錄都刪除 可以用這個指令救回
git restore  .   檔案或目錄刪除也可以用restore這個指令救回
git branch       檢視分支
git branch 名稱   建立分支
git switch 檔案名稱  切換分支
git blame 檔案名稱   找出檔案程式碼哪一行是誰寫的
git merge         合併分支

checkout可以救回檔案也可以切換分支，避免混淆
所以有了 restore 和switch 更容易辨別


git log 可以看到歷史紀錄
git log --oneline
建議裝外掛 git graph
(vscode也有 view --->source control )


### branch 分支
* 是HEAD 上帝視角
- 分支只是一張貼在某個Commit上的貼紙
- 分支有 main master

#### merge合併
- 合併分支，要先用git switch切換控制權，再git merge 分支， 控制權會往前移
- 如果 git merge 控制權，終端機會顯示最新狀態
- merge，可以保留歷史紀錄，節點合併節點越多，越混亂



有分支交流道
git merge xx --no-ff -m ""
git blame 檔案名稱

rebase（不想保留歷史紀錄 節點相對單純直接）
reset

快轉（Fast-forward） 合併

<!-- learn git -->


--mixed
--soft
--hard

^  ~
git reset head^ --hard

<!-- ssh -->
git push
git pull = git fetch + git merge
git pull --rebase=git fetch+auto git rebase

git clone 

GitHub  
