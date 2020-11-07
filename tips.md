# 怎么用github做项目展示

## master

初始化版本库，用于生成.git文件

```sh
git init
```

将所有文件添加到缓存区

```sh
git add .
```

提交当前工作空间的修改内容

```sh
git commit -m "first commit"
```

将仓库连接到远程服务器

```sh
git remote add origin <server>
```

将改动推送到所添加的服务器上

```sh
git push -u origin master
```

## gh-pages

初始化版本库，用于生成.git文件

```sh
git init
```

将仓库连接到远程服务器

```sh
git remote add origin <server>
```

新建并切换到gh-pages分支

```sh
git checkout --orphan gh-pages
```

之后的操作和之前一样，只是push到gh-pages分支而不是默认的master

```sh
git add . 
git commit -m "update"
git push -u origin gh-pages
```

# git 常用命令

…or create a new repository on the command line

```sh
echo "# aa-" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:kakapiya/aa-.git
git push -u origin master
                
```

…or push an existing repository from the command line

```sh
git remote add origin git@github.com:kakapiya/aa-.git
git push -u origin master
```