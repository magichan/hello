### git 基本操作 
git status 用来查看结果
git diff 查看修改了什么
git log 显示最近的提交信息
  显示的内容中比较重要的是唯一的编码(SHA1计算的值),和commit 时添加的评论

git 使用　`HEAD` 表示当前版本,上一版本为`HEAD^`,再上一版本为`HEAD^^`
同时使用 `git reset` 来回退版本
```
git reset --hard HEAD^
```
使用同样的命令，利用ID，不仅可以往后退，也可以从回退后的版本，返回到原版本，即往前退
至于id,可以利用记录你每一次命令的 `git reflog` 来操作

### 工作区和暂存区

