# 常用操作合集

## 分支清理
```shell
# 删除远程已删除分支的引用
git fetch -p
# 删除除当前分支的所有本地分支
git branch | grep -v '\*' | xargs git branch -D


```