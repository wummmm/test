# 我也不知道写点啥...
#查看日志
git log 查看历史提交的日志
git log --oneline 可以看到简洁版的日志

# 回退到指定的版本
git reset --hard Head~0
表示回退到上一次代码提交时的状态
git reset --hard Head~1
表示回退到上上次代码提交时的状态
git reset --hard [版本号]
可以通过版本号精确的回退到某一次提交时的状态
git reflog
可以看到每一次切换版本的记录:可以看到所有提交的版本号

##分支
默认是有一个主分支的master
###创建分支
git branch dev
创建了一个dev分支
在刚创建时dev分支里的东西和master分支里的东西是一样的
###切换分支
git checkout dev
切换到指定的分支,这里的切换到名为dev的分支
git branch 可以查看当前有哪些分支
### 合并分支
git merge dev
当前分支内容,吧当前分支与指定的分支(dev),进行合并
当前分支指的是git branch 命令输出的前面有*号的分支
合并时如果有冲突，需要手动去处理，处理后还需要在提交一次.
