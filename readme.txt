git is version control system
git status 用来查看结果
git diff 查看修改了什么
git log 显示最近的提交信息
  显示的内容中比较重要的是唯一的编码(SHA1计算的值),和commit 时添加的评论

git 使用　`HEAD` 表示当前版本,上一版本为`HEAD^`,再上一版本为`HEAD^^`
同时使用 `git reset` 来回退版本
```
git reset --hard HEAD^
```

