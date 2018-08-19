# git常用指令
## 一.当前文件目录添加到git环境
1. git init   使当前目录添加到git管理
2. git add test   把test文件夹添加到git管理， . 点表示当前目录下的所有文件夹全部添加到git管理中
3. git commit -m "提交说明"   把当前在git管理中的文件提交到本地库中，提交说明一定要写。
4. git remote add origin "url"  当前文件夹联结到仓库，ulr 为你要联结的仓库地址。
5. git push -u origin master  把工程上传到git,会弹出输入框输入用户名和密码

## 二.从git仓库下载工程到本地
1. git clone "url" 把仓库里面的工程克隆到当天文件夹
2. git clone "url" <本地目录名>
3. git checkout "0.1" 把当前工程切换到0.1这个版本

## 三. Git branch
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

## 五. 
