# eeui登录插件 

只支持安卓  

目前支持以下第三方登录，持续扩展中：  
微信登录  
微博登录   


使用步骤：  
  
一.在项目根目录执行下面语句：  
```javascript
  eeui plugin create openlogin
```
  
二.下载压缩包后，打开 根目录\plugins\android 文件夹；替换掉 openlogin  

三.用android studio 打开项目  

1.修改包名为你的项目包名，如图：  
![image](https://raw.githubusercontent.com/netzhouxiang/eeui-openlogin/master/1.png)  
![image](https://raw.githubusercontent.com/netzhouxiang/eeui-openlogin/master/2.png)  

2.增加新浪微博支持：  
```javascript
  maven { url "https://dl.bintray.com/thelasterstar/maven/" }
```
![image](https://raw.githubusercontent.com/netzhouxiang/eeui-openlogin/master/3.png)  
  
  
3.修改你的微信应用ID和微博应用配置  
![image](https://raw.githubusercontent.com/netzhouxiang/eeui-openlogin/master/4.png)  

4.在项目中，通过以下代码调用：  
```javascript
  const ol = app.requireModule('openlogin');
  //微信登录
  ol.login(res=>{
    //res回调
  });
  //微博登录
  ol.weibologin(res=>{
    //res回调
  });
```