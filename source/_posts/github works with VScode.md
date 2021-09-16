---
title: github works with VScode
hidden: true
author: 柴祥
---
#用VScode在github上做项目

-以Arch为例



1. 下载并安装vscode
 ``` shell
    sudo pacman -S vscode
```
输入Y,表示确认

pppppppppppppppppp

2. 打开vscode

打开桌面最左下菜单找vscode,或在文件管理/home找vscode的文件中点击可执行文件打开

3. 装上vscode的所需插件来让它成为你工作

以下以我习惯的必用插件为例子：CodeLLDB、 clangd(编译器插件)、   GitLens-Git supercharged（辅助github工作的插件）、  Chinese (Simplified) Language（非必须，设置成中文的插件）

ppppppppppppppppppppppppppp

记得重启软件

4. 申请github账号

5. 创建一个github仓库

- Repository name 这取一个仓库名

- Description (optional) 让你描述一下这个仓库是干什么的

- Public 设为公开（跟你朋友圈一样，让不让别人看）

- Private 设为隐私

- Add a README file （添加一个README文件，类似于B站的视频的简介，也是介绍你这是在搞什么东西）
- Add .gitignore  （Git忽略文件.gitignore的使用）
- Choose a license  （LICENSE，许可证，别人使用你这仓库里的东西时要遵守的条款，可能会侵权）

6. 已完成创建一个仓库！

**注**：以下操作可以在vscode自带的Terminal完成
包括命令大多都可以用图形化的操作代替


**注**：以下所有操作都需要完成SSH Key先

7. 克隆你的仓库
```
git clone 你的仓库链接
如： git clone git@github.com:chaixiang2002/helloworld.git
```
你的仓库链接在网站的这里
ppppppppppp

图形化的操作：

8. 修改后将工作区提交到暂存区
```
git add 文件名
如： git add -A     (所有文件都提交)
```

9. 暂存区提交到仓库
```
git commit -m "介绍你的提交内容的话"
```

10. 创建与合并分支
有时一个项目会向多个方向发展，我们可以创建一个新的分支(没创立分支前，默认在主分支{master}工作)

```
git checkout  -b '分支名'
```
切换到某分支工作
```
git checkout 分支名
```
把a分支合并到主分支上
```
git merge 分支名
```
放弃合并
```
git merge --abart
```





11.  将本地仓库上传的github远程仓库(**此操作要先链接到github远程仓库**)

链接到github远程仓库
```
git remote add origin 该远程仓库的链接
```
上传到远程仓库
```
git push -u origin master
```
12. 更新本地仓库与网站上一致
```
git pull origin 分支名
```

13. （非必要但是常识）将普通文件夹初始化成本地仓库
```
git init 
```









