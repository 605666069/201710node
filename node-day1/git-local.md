## git本地操作
- 不停的创造文件进行备份(没有修改的提示) git可以帮我们管理我们的代码保证代码不丢失
- 记录历史只要代码提交到git上就永久不会丢失，可以随时“穿越”
- 团队协作 俩个人修改了同一个文件的同一行，也需要手动解决冲突，可以实现自动合并 （模块化，组件化）
- git拥有强大“分支”管理系统

## 分布式
- svn(集中式) 需要一台中央服务器
- git的区别
- 速度比svn快
- svn中每个文件夹都有一个文件.svn文件，git有一个单独的文件.git文件夹

## git安装
- windows http://git-scm.com
- mac 如果安装过xcode自带git，homebrew是wmac的包管理器
- http://ohmyz.sh/
- http://www.iterm2.com/

## 配置用户(不配置用户不能提交代码)
```
git config --list
git config --global user.name "你的名字"
git config --global user.email "你的邮箱"
```

## 初始化git
- 一个项目初始化一次，不能嵌套
```
git init 告诉git哪个文件夹被git所管理
git status 查看git状态
```

## 删除暂存区
```
git rm --cached 文件名
```

## 添加到暂存区
```
git add ./ -A / 文件名
```

## 添加到历史区
```
git commit -m '消息'
```

## git的对比
- git diff 工作区和暂存区
- git diff 分支名 工作区和历史区
- git diff --cached 暂存取和历史区比较

## 撤销
- 从暂存区中将工作区内容覆盖掉
```
git checkout 文件名
git reset HEAD 文件名 回到上一次的缓存区
```

## 回滚历史版本
```
git reset --hard 版本号
git reflog 查看所有版本
```

## 回滚某个版本的文件
```
git checkout 版本号 文件名
```

## 创建分支
```
git branch 分支名
git branch 查看分支
```

## 切换分支
```
git checkout 分支名
```

## 删除分支
```
git branch -D 分支名
```

> 删除分支时当前用户不能在当前要删除的分支上

## 创建并切换分支
```
git checkout -b dev
```

> 添加文件到历史区此时两个分支就没关系了

## 文件修改切换分支
```
git stash 暂存文件
git stash pop 还原暂存的内容
```

> 分支有更改不能直接切换，可以提交更改或者暂存更改，暂存使用过渡区覆盖掉工作

## 合并分支
```
git merge 分支名
```

## echo输入文件内容
```
echo '内容' >> 1.txt
```

## 解决冲突
- 遇到冲突时只能手动的解决冲突，留下想要的结果再次提交

## 推送到github


## linux命令
- pwd print working directory
- rm -rf 文件夹 删除文件
- rm 文件名 删除文件
- mkdir 文件夹名字 创建目录
- cd 目录名 change directory
- ls -al显示目录下所有的文件
- touch 文件名 创建文件
- cat 文件名
- vi 文件名
 - i:插入模式 esc退出编辑模式 :q!强制退出 :wq 保存并退出

http://man.linuxde.net/vi
