# Git常用命令

### 1. git init

初始化当前文件夹为git管理的文件夹

```
git init
```

当前目录下新建directory文件夹，并初始化directory文件夹为git管理的文件夹

```
git init [directory]
```

### 2. git add

将当前目录下（及子目录下）未被git管理的文件及文件夹加入到git管理中

```
git add .
```

### 3. git commit

提交暂存区文件到本地仓库，提交信息必填

```
git commit -m "msg"
```

### 4. git remote

列出所有远程仓库的简写（shortName）

```
git remote
```

列出所有远程仓库

```
git remote -v
```

添加远程仓库

```
git remote add <name> <url>
```

### 5. git branch

注意：Git的分支只有在有提交后，才可以使用git branch命令看到，原理未知，猜测分支必须指向一次提交，初始化仓库后，没有任何一次提交，因此分支无法显示。

列出所有本地分支

```
git branch
```

列出所有本地分支和远程分支

```
git branch -a
```

查看本地分支和远程分支的映射关系

```
git branch -vv
```

将本地分支和远程分支相关联（仅上行）

```
git branch --set-upstream <local branch> <remote branch>
```

### 6. git push

推送当前分支到远程仓库分支（需要有映射关系）

```
git push
```

推送本地分支到远程分支

```
git push [<repository> [local branch]:[remote branch]]
```

### 7. git fetch

获取远程仓库信息

```
git fetch <remote>
```

