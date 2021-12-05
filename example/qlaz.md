青龙面板小白傻瓜安装教程
-------
一、需要的工具：
-------
* 云服务器：建议1核1G以上配置，选CentOS 8系统，云服务器阿里云.腾讯云都可以，一般新用户买1年几十块<br>
* ssh链接工具：用来连接服务器来输入命令的，我用的FinalShell  [点击下载](http://www.hostbuf.com/downloads/finalshell_install.exe)<br>

二、安装docker<br>
-------
1、安装命令如下：

    curl -fsSL https://get.docker.com | bash -s docker --mirror Aliyun
 也可以使用国内 daocloud 一键安装命令：

    curl -sSL https://get.daocloud.io/docker | sh


