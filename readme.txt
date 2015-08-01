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


### 分支学习


一条完整的时间线作为一条分支，而最初始的分支被一般被称为　`master` 分支，　严格来说　`HEAD` 指向的是　
当前分支，即正在操作的分支，所以当创建新的分支时，就会　`HEAD`　就会跑到操作分支上

`git branch dev`  创建 `dev` 分支
`git checkout dev` 切换到　`dev` 分支
以上两个命令等价于　

`git checkout -b dev ` 代表创建一个 `dev` 分支，而参数意味着创建并切换分支

`git branch ` 查看分支，当前分支用 `*` 标明　

`git merge name` 用于指定分支合并到当前分支

`git branch -d name ` 删除指定分字
