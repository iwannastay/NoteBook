# 常用操作合集

## 本地分支清理
```shell
# 删除除当前分支的所有本地分支
git branch | grep -v '\*' | xargs git branch -D

# 更新本地的远程分支引用，清理已经被删除的远程分支的本地引用
git fetch -p --all 

# 拉取并合并所有远程仓库的更新到当前本地分支
git pull --all

```

## 重置个人仓
```shell
git checkout master
git reset --hard up/master
git push origin master -f

```