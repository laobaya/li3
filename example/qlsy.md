
## 一、开打青龙面板：iP:5700，点击右上角的添加任务

* 名称可以随意填写，命令填写大佬们的拉库命令或者单个脚本拉取命令 例如拉取`faker2`仓库

  1、名称（可以随意填写）
 
      faker2仓库

  2、faker2仓库拉库命令
  
       ql repo https://ghproxy.com/https://github.com/shufflewzc/faker2.git "jd_|jx_|gua_|jddj_|getJDCookie" "activity|backUp" "^jd[^_]|USER|function|utils|sendNotify|ZooFaker_Necklace.js|JDJRValidator_|sign_graphics_validate|ql"
       
   3、定时 （按照你需要的定时格式写，不会就填下面这个）  
   
       2 0-23/4 * * *
![](https://github.com/z115870/li3/blob/main/img/12.png)

* 点击确定，然后点击运行

![](https://github.com/z115870/li3/blob/main/img/13.png)

* 等待一会儿，运行完成以后刷新浏览器，就可以看到`faker2`仓库的脚本都被拉取下来了

![](https://github.com/z115870/li3/blob/main/img/14.png)

## 二、脚本已经拉好了，该怎么给我们自己账号做任务呢？那就需要抓我们账号的COOKIE。

* 抓取COOKIE方式有很多种,先用下比较原始的方法

   1、打开浏览器，输入网址，在点击登录，用手机验证码登录，这样验证码登录有效期可以一个月左右。
   
      m.jd.com
      
   2、然后按`F12`，打开控制台，找到`网络`再找到`newhome.action`这一行点开，可以看到右边往下滑能看到有`cookie: `后面还有一大串，我们在这里面找到pt_key=xxx;pt_pin=xxx;这个量就是我们要的ck，  不懂看图（复制的pt_key和pt_pin中间有一个空格记得去了）
