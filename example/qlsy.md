
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
      
   2、然后按`F12`，打开控制台，找到`网络`再找到`newhome.action`这一行点开，可以看到右边往下滑能看到有`cookie: `后面还有一大串，我们在这里面找到`pt_key=xxx;pt_pin=xxx;`这个量就是我们要的ck，不懂看图（复制的pt_key和pt_pin中间有一个空格记得去了）
   
   ![](https://github.com/z115870/li3/blob/main/img/16.png)
   
   3、把我们找到的`pt_key=xxx;pt_pin=xxx;`复制下来，再次打开青龙面板，点左边的`环境变量`，再点右上角的`添加变量`，名称填`JD_COOKIE`这个不能填错，
值就填我们复制好的`pt_key=xxx;pt_pin=xxx;`（再重申：pt_key和pt_pin中间有一个空格记得去了），然后备注可以填写谁谁的账号以免忘记，填好后点击确定

![](https://github.com/z115870/li3/blob/main/img/17.png)

至此，拉取的脚本到了设定的时间点就会运行，就会给我们脚本做任务了。

## 三、添加依赖，如果不添加依赖，很多脚本运行时会报错，不能正常使用

* 打开青龙面板，找到左边依赖管理，再点右上角添加依赖就可以了,把以下依赖挨个添加就可以了

NodeJs依赖：   

`crypto-js`  
`crypto -g`  
`jsdom`  
`upgrade`  
`pip`  
`tslib`  
`png-js`  
`date-fns`    
`@types/node`    
`requests`  
`axios`  
`js-base64`  
`upgrade`   
`pip`  
`npm`  
`md5`  

Python3依赖：

`aiohttp`      
`requests`    
`jieba`   



