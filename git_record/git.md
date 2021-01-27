git checkout . 删除本次所有操作

git status 查看本次修改状态

git stash 暂存本次修改

git stash pop 复原暂存操作

git stash clear 清除所有队列

git stash drop stash@{0} 清除第一个队列

git pull origin [branch] 拉取别的分支代码合并(不知道是不是本公司配置了啥)

git push origin --delete [branchname] 删除远端分支

git tag 查看所有 tag

git tag [tagname] 新建一个 tag

git tag -d tag_name 删除单个 tag

git push origin [tagname] 单个 tag 推送到远端

git push origin --tags 全部 tag 推送到远端

git commit --no-verify -m "提交" //可以跳过代码检查
