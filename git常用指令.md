# git常用指令
## 一.当前文件目录添加到git环境
1. git init   使当前目录添加到git管理
2. git add test   把test文件夹添加到git管理， . 点表示当前目录下的所有文件夹全部添加到git管理中
3. git commit -m "提交说明"   把当前在git管理中的文件提交到本地库中，提交说明一定要写。
4. git remote add origin "url"  当前文件夹联结到仓库，ulr 为你要联结的仓库地址。
5. git push -u origin master  把工程上传到git,会弹出输入框输入用户名和密码
6. git commit -a 把当前所有的文件添加到git管理并且提交
7. git rm 删除文件（从git版本库中移除）
8. git -f 删除文件（强制删除，不能被git恢复）
9. git mv old_name new_name 移动文件

## 二.从git仓库下载工程到本地
1. git clone "url" 把仓库里面的工程克隆到当天文件夹
2. git clone "url" <本地目录名>
3. git checkout "0.1" 把当前工程切换到0.1这个版本

## 三.分支 Git branch
1. git branch  列出本地已经存在的分支，并且在当前分支的前面用"*"标记
2. git branch -a 查看当前的所有分支
3. git branch -r 查看远程本库分支列表
4. git branch dev 创建dev分支，创建分支时需要是最新的环境，创建分支但依然停留在当前分支
5. git branch -d dev 删除dev分支，如果在分支中有一些未merge的提交，那么会删除分支失败，此时可以使用 git branch -D dev：强制删除dev分支
6. git branch -vv 可以查看本地分支对应的远程分支
7. git branch -m oldName newName 给分支从新命名

## 四. Git checkout
1. git checkout filename 放弃单个文件的修改
2. git checkout . 放弃当前目录下的修改
3. git checkout master 将分支切换到master
4. git checkout -b master 如果分支存在则只切换分支，若不存在则创建并切换到master分支

## 五. 状态 git status
1. git status 查看当前文件的状态
2. git add README.md 暂存已修改的文件
3. git status -s 状态简览

## 六. cat .gitignore 忽略不必要的文件提交
1. http://github.com/github/gitignore 查看已经配置好的忽略项
2. 把.gitignore 文件放在需要过滤的文件夹内，该文件夹下的所有文件都在过滤的目标范围内

## 七. git diff 查看已暂存和未暂存的修改
1. git diff --cached 查看已经暂存起来的变化

## 八. git commit --amend 撤销操作
1. 提交命令尝试重新提交
2. 将暂存区中的文件提交，提交过了不提交，没有提交或者修改过的会提交

## 九. 

