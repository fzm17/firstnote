git config --global user.name "ahen"
git config --global user.email "ahen@xxx.yyy"
# initial
git init

git status
# 查看現在狀態

git add . (*.md) (filename)
# 將所有檔案加入暫存區 (把所有md結尾的檔案加入) (把特定filename加入)

git commit -m "name"
# 將暫存區的檔案加入到本地端的版本庫

git log (--oneline)
# 查看版本庫的歷史紀錄 (只顯示一行)

git diff ("parameter")
# 查看檔案的差異 (parameter: 版本號，可於git log查看)

git checkout ("parameter") (filename)
# 切換到特定版本 (parameter: 版本號，可於git log查看) (切換到特定檔案的特定版本，不會影響其他檔案，如果沒有指定檔案，則會切換到該版本的所有檔案)

git checkout master
# 切換到最新版本

git reset --hard ("parameter")
# 回到特定版本 (parameter: 版本號，可於git log查看)

如果包含移除檔案 同樣需要執行一次git add . 才能commit
如果有不想變動的檔名(檔案)，可以在工作目錄建立 .gitignore 並寫於裡面來忽略