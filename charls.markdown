# charles抓包工具小试牛刀

## charles的简介

换了mac之后，抓包工具charles代理了以前各种wireshark、fiddler等windows环境下的抓包工具。通过唐巧博客的分享和工作中的熟悉与运用，这个抓包工具代替了小半个数据库权限一般，测试的时候再也不用依赖服务器的同学帮助了。(本文以charles4.0.2为例)

对于测试同学来说，charles的主要功能：

1.截取http和http网络封包。
2.大量重发网络请求做一个压力测试。
3.修改请求参数,返回极限case想要的结果。
4.模拟慢速网络。
5.更强大功能等待实践中发现...

## charls的安装
当然，不是破解版的charles会让人很奔溃，启动延时,抓包30分钟就会强制关闭!这里提供两个下载途径：
1.官网可下载（http://www.charlesproxy.com）
2.这边提供mac的破解版
安装步骤：
1.打开后缀dmg的镜像（即将其拖至Application目录下即可）。
2.找到Mac的
Finder>>应用程序>>右键显示包内容>>contents/Java路径下的charles.jar文件，用包内的jar文件将其替换。
3.打开charls，菜单栏中找到“Help-Register Charles”，输入任意信息即可完成注册。

## charles视图简介
安装完成，让我们一起看下它的首页，如下图：

[!img](https://i.loli.net/2017/08/22/599c44f537383.jpeg
)

charles的Filter功能可以过滤某种host或是url的某个字段；右键选中某个host点击focus，主界面选中过滤栏的focused，会自动筛选出该host的所有请求，常用于不知道关键字的一些请求。响应内容会有JASON格式，内容为图片也可以预览。

## 截取移动端的http和https请求

### 各种各样的settings

http请求不需要安装证书，而https是需要安装证书的。
首先，安装charles上的证书：

[!img](https://i.loli.net/2017/08/22/599c4a7fc8e05.jpeg)

按步骤安装证书并信任。

其次，安装移动端的证书：
