1. 安装npm，从网站 下载node.js源代码 [https://nodejs.org/\#download](https://nodejs.org/#download) 

```
解压
./configure

make
make
 install
```

成功执行后，npm就被安装好了。

1. gitbook 安装  222

```
npm
 install -g gitbook-cli
```

```
gitbook
 -V
```

查看gitbook是否安装成功。

3 安装git

[https://code.google.com/p/msysgit/downloads/list](https://code.google.com/p/msysgit/downloads/list)

4 生成sshkey

输入 ssh-keygen ，按enter，一直按enter 公钥生成在 C:\Documents and Settings\xxx.ssh 目录中，找到目录 ，里面有id\_rsa.pub文件，用记事本打开，然后把里面的东西 全选复制。

并在github上配置sshkey

5 下载gitbookeditor并安装

[https://www.gitbook.com/editor/windows](https://www.gitbook.com/editor/windows)

6 github上新建一个项目

git@github.com:zimingforever/mygitbook.git

并把这个项目直接clone到gitbook的文件目录下面C:\Users\XXX\GitBook\Library\Import\mygitbook

初始化文件夹

```
echo
# mygitbook 
>
>
 README.md

git initgit add README.md
git commit -m 
"first commit"

git remote add origin git
@github
.com:zimingforever/mygitbook.git
git push -u origin master
```

7 打开gitbookeitor，FILE-》imoport 找到之前的clone的文件

左侧table of contents可以增加新的章节或者文章

8 gitbook editor打开后，book-editor confugration可以设置book.json文件

9 目录 book-repo setting可以设置远程的git地址，需要更改成http的地址[https://github.com/zimingforever/mygitbook.git](https://github.com/zimingforever/mygitbook.git)，然后设置对应的账号及密码

10 每次gitbook eidtor编辑完之后可以点击下右侧的sync按钮，相关的文件就会推到github上

11 使用gitbook命令生成对应的html文件

```
c:


cd 
C:
\Users\xxx\GitBook\Library\Import\

gitbook build mygitbook
```

12 将生成好的html文件推到github上

```
c:


cd 
C:
\Users\xxx\GitBook\Library\Import\mygitbook

git config --global credential.helper store

git add -A

git commit -m 
'udpatebook'


git push

start 
https:
//github.com/zimingforever/mygitbook/tree/master/_book
```

13 GITBOOK editor的使用界面

![](http://static.oschina.net/uploads/space/2016/0104/102601_0wYV_195637.png)

14 使用githubpage来打开对应的地址

[http://htmlpreview.github.io/](http://htmlpreview.github.io/)

15 生成地址为[http://htmlpreview.github.io/?https://github.com/zimingforever/mygitbook/blob/master/\_book/index.html](http://htmlpreview.github.io/?https://github.com/zimingforever/mygitbook/blob/master/_book/index.html) 直接访问即可

![](http://static.oschina.net/uploads/space/2016/0104/103402_RImP_195637.png)

