---
published: false
---
# 关闭Windows休眠、怎么删除hiberfil.sys占用空间
版权声明：本文为转载文章。
本文链接：[https://jingyan.baidu.com/article/22a299b5f6f4809e18376a5b.html](https://jingyan.baidu.com/article/22a299b5f6f4809e18376a5b.html)

前言：如何关闭开始菜单的休眠？本教程适合winodws 10 和windows 7的用户，我是以win10系统为例的，但win关闭休眠的方法和win10基本上是一样的呢~

1.  windows10/7系统盘中，隐藏文件【hiberfil.sys】占据C盘3.17G的空间，特别是有些用户安装的固态硬盘本来就不大，因此关闭休眠很有必要

    ![windows10\7关闭休眠，怎么删除hiberfil.sys](https://exp-picture.cdn.bcebos.com/def72c6c576699cf54094fd7a885e036e3915ef2.jpg?x-bce-process=image%2Fresize%2Cm_lfit%2Cw_500%2Climit_1)

2.  在桌面按快捷键【WIN+R】打开运行窗口，输入【cmd】，然后点【确定】打开【命令提示符】

    ![windows10\7关闭休眠，怎么删除hiberfil.sys](https://exp-picture.cdn.bcebos.com/32a127723d03bbea5edc50fcea43d7d4493154f2.jpg?x-bce-process=image%2Fresize%2Cm_lfit%2Cw_500%2Climit_1)

3.  在打开的【命令提示符】页面直接输入【powercfg -h 0ff】（注意有空格）

    然后点击回车键【Enter】

    ![windows10\7关闭休眠，怎么删除hiberfil.sys](https://exp-picture.cdn.bcebos.com/05aae8a75f0f822b1db47c86c018512c8df14df2.jpg?x-bce-process=image%2Fresize%2Cm_lfit%2Cw_500%2Climit_1)

4.  如果出现这个，证明已经成功关闭休眠啦~

    ![windows10\7关闭休眠，怎么删除hiberfil.sys](https://exp-picture.cdn.bcebos.com/d9e638334884cde33976365af07f860e7d7542f2.jpg?x-bce-process=image%2Fresize%2Cm_lfit%2Cw_500%2Climit_1)

5.  我们可以看到【开始】菜单的关机按钮里，已经没有【休眠】选项了

    ![windows10\7关闭休眠，怎么删除hiberfil.sys](https://exp-picture.cdn.bcebos.com/e4b5e2f5ee0d3aced18d12df87e265e7350fbbf2.jpg?x-bce-process=image%2Fresize%2Cm_lfit%2Cw_500%2Climit_1)

6.  原本在C盘的隐藏文件【hiberfil.sys】也消失了

    ![windows10\7关闭休眠，怎么删除hiberfil.sys](https://exp-picture.cdn.bcebos.com/65390a23beb9763ea598db626ad06de89b61b0f2.jpg?x-bce-process=image%2Fresize%2Cm_lfit%2Cw_500%2Climit_1)

7.  但如果我们在【命令提示符】中,输入【powercfg -h off】提示出现错误（0×65b）,证明我们不是以管理员运行命令提示符的，那我们就要通过管理员来关闭休眠了

    ![windows10\7关闭休眠，怎么删除hiberfil.sys](https://exp-picture.cdn.bcebos.com/87645f93cee8b004d941b1bb79260d9a300ea9f2.jpg?x-bce-process=image%2Fresize%2Cm_lfit%2Cw_500%2Climit_1)

8.  鼠标右键点击左下角【开始】，

    再点击【命令提示符(管理员)】

    ![windows10\7关闭休眠，怎么删除hiberfil.sys](https://exp-picture.cdn.bcebos.com/e86ba4b842406afe544e91711eee41c1b6279ff2.jpg?x-bce-process=image%2Fresize%2Cm_lfit%2Cw_500%2Climit_1)

9.  这次打开的就是管理员模式的命令提示符啦，再次输入【powercfg -h 0ff】就可以关闭休眠啦~

    ![windows10\7关闭休眠，怎么删除hiberfil.sys](https://exp-picture.cdn.bcebos.com/07c98f2ca5cadce831126048fcf7980e5e2095f2.jpg?x-bce-process=image%2Fresize%2Cm_lfit%2Cw_500%2Climit_1)

10.  如果想再打开休眠，可以输入【powercfg -h on】,是不是很简单呀~只要我们记住这两个命令，就方便更改休眠设置了

    ![windows10\7关闭休眠，怎么删除hiberfil.sys](https://exp-picture.cdn.bcebos.com/589f5b0788013870661b5a382d08a50f95fc83f2.jpg?x-bce-process=image%2Fresize%2Cm_lfit%2Cw_500%2Climit_1)
