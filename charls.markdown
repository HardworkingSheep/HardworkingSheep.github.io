# charles抓包工具小试牛刀

## charles的简介

换了mac之后，抓包工具charles代理了以前各种wireshark、fiddler等windows环境下的抓包工具。通过唐巧博客的分享和工作中的熟悉与运用，这个抓包工具代替了小半个数据库权限一般，测试的时候再也不用依赖服务器的同学帮助了。

对于测试同学来说，charles的主要功能：

1.截取http和http网络封包。
2.大量重发网络请求做一个压力测试。
3.修改请求参数,返回极限case想要的结果。
4.模拟慢速网络。
5.更强大功能等待实践中发现...

## charls的安装
当然，不是破解版的charles会让人很奔溃，启动延时，抓包30分钟就会强制关闭!这里提供两个下载途径：
1.官网可下载（http://www.charlesproxy.com）
2.这边提供mac的破解版
安装步骤：
1.打开后缀dmg的镜像（即将其拖至Application目录下即可）。
2.找到
Finder>>应用程序>>右键显示包内容>>contents/Java路径下的charles.jar文件，用包内的jar文件将其替换。
3.打开charls，菜单栏中找到“Help-Register Charles”，输入任意信息即可完成注册。

## charles视图简介
