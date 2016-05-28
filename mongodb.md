##首先到[官网](http://www.mongodb.org/downloads )下载合适的安装包，目前的最新版本为2.6
![mahua](mahua-logo.jpg)
##基本安装配置和相关目录
###在D盘创建MongoDB文件夹
下载后注意安装的时候路径的选择
* 解压安装包到D:\MongoDB
* 建立数据库目录 D:\MongoDB\data
* 建立日志目录 D:\MongoDB\logs
* 建立配置文件目录 D:\MongoDB\etc
* 建立配置文件 D:\MongoDB\etc\mongodb.conf

```code
    dbpath=D:\MongoDB\data #数据库路径
    logpath=D:\MongoDB\logs\mongodb.log #日志输出文件路径
    logappend=true #错误日志采用追加模式，配置这个选项后mongodb的日志会追加到现有的日志文件，而不是从新创建一个新文件
    journal=true #启用日志文件，默认启用
    quiet=true #这个选项可以过滤掉一些无用的日志信息，若需要调试使用请设置为false
    port=27017 #端口号 默认为27017
```
控制台切换D:\MongoDB\bin 执行
```code
    mongod --dbpath D:\MongoDB\data
```
如果出现
```code
2016-05-28T16:53:26.510+0800 I CONTROL  [initandlisten] MongoDB starting : pid=257920 port=27017 dbpath=D:\MongoDB\data 64-bit host=l
……
```
success!!!!
##进阶
把它注册为window服务，这样每次不用回到命令行输入命令

配置文件和相关目录建好后使用如下方式启动MongoDB
* 普通启动
```code
    mongod --config D:\MongoDB\etc\mongodb.conf
```
* 安装为window服务
    
```code
    mongod --config D:\MongoDB\etc\mongodb.conf --install
``` 
##有问题反馈
在使用中有任何问题，欢迎反馈给我，可以用以下联系方式跟我交流

* 邮件(duleigiser#126.com, 把#换成@)
* QQ: 564779666
* weibo: [@duleigiser](http://weibo.com/u/2356693923)

##捐助开发者
在兴趣的驱动下,写一个`免费`的东西，有欣喜，也还有汗水，希望你喜欢我的作品，同时也能支持一下。
当然，有钱捧个钱场（右上角的爱心标志，支持支付宝和PayPal捐助），没钱捧个人场，谢谢各位。

##感激
感谢以下的项目,排名不分先后

* [懒惰的肥兔](http://www.cnblogs.com/lzrabbit/p/3682510.html) 


##关于作者

```javascript
  var ihubo = {
    nickName  : "杜磊",
    site : "https://www.github.com/duleigiser"
  }
```
