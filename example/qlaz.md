# 青龙面板小白傻瓜图文安装教程

## 一、需要的工具：

* 云服务器：建议1核1G以上配置，选CentOS 8系统，云服务器阿里云.腾讯云都可以，一般新用户买1年几十块<br>
* ssh链接工具：用来连接服务器来输入命令的，我用的FinalShell  [点击下载](http://www.hostbuf.com/downloads/finalshell_install.exe)<br>

## 二、连接服务器：

* 打开FinalShell：

![](https://github.com/z115870/li3/blob/main/img/1.png)
![](https://github.com/z115870/li3/blob/main/img/2.png)
![](https://github.com/z115870/li3/blob/main/img/3.png)
![](https://github.com/z115870/li3/blob/main/img/4.png)

完毕！
## 三、安装docker

* 可以按照菜鸟教程安装：[点击跳转](https://www.runoob.com/docker/centos-docker-install.html)<br>
* 安装好docker后我们可以检查下是否安装成功 输入命令：

      docker version
      
![](https://github.com/z115870/li3/blob/main/img/5.png)
![](https://github.com/z115870/li3/blob/main/img/6.png)
  
完毕！  
## 三、安装好docker后我们开始安装青龙面板

* 拉取青龙面板镜像，把命令输入到shh回车等待完成

      docker pull whyour/qinglong:latest
      
![](https://github.com/z115870/li3/blob/main/img/7.png)      
      
* 镜像拉取成功后启动容器
   
      docker run -dit \
         -v $PWD/ql/config:/ql/config \
         -v $PWD/ql/log:/ql/log \
         -v $PWD/ql/db:/ql/db \
         -v $PWD/ql/scripts:/ql/scripts \
         -p 5700:5700 \
         --name qinglong \
         --hostname qinglong \
         --restart always \
         whyour/qinglong:latest     
         
![](https://github.com/z115870/li3/blob/main/img/8.png)         

完毕！
## 四、容器启动成功后，打开浏览器输入：服务器IP:5700 ,然后开始设置青龙面板信息

![](https://github.com/z115870/li3/blob/main/img/9.png)
![](https://github.com/z115870/li3/blob/main/img/10.png)

## 至此，青龙面板已经安装成功！

* 欢迎小白们加企鹅群交流：891180955
