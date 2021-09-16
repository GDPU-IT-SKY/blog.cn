---
title: Linux github 教程
hidden: true
author: 柴祥
---
### 命令行是什么？（终端/ Terminal）
快捷键:  Ctrl+Alt+T
你输入什么命令
及








### SSH Key
这是你电脑生成的一个钥匙，提交给github,是让github记住你的设备,用terminal（终端）完成

1、首先在本地创建ssh key
```
$ ssh-keygen -t rsa -C "你的github账号绑定的邮箱"
```

ppppppppppppppppppppppppppppp1

然后一直按确认（回车）

成功的话会在~/下生成.ssh文件夹，进去，打开id_rsa.pub，复制里面的key。

**notice**:.ssh

ppppppppppppppppppppp

回到github上，进入 Account Settings（账户配置），左边选择SSH Keys，Add SSH Key,title随便填，粘贴在你电脑上生成的key。

ppppppppppppppppppppppppppp

2、验证是否成功（可跳过）
为了验证是否成功，下输入： 
```
$ ssh -T git@github.com
```
如果是第一次的会提示是否continue，输入**yes**就会看到：You've successfully authenticated, but GitHub does not provide shell access 。这就表示已成功连上github。 

3、设置username和email

接下来我们要做的就是把本地仓库传到github上去，在此之前还需要设置username和email，因为github每次commit都会记录他们。 
```
$ git config --global user.name "your name"
$ git config --global user.email "your_email@youremail.com"
```


到这步，ssh key就完成了
