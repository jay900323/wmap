# wmap
## 介绍
Web指纹也叫web应用指纹。由于所使用的工具、技术、实现方式等因素的影响，每个web网站都形成了一些独有的特点，我们把这样的特点叫做web应用指纹。

例如：
1、百度百科网站使用了Apache web服务器<br>
2、网易网站使用了Nginx web服务器<br>
3、补天平台使用了ThinkPHP框架<br>

以上内容都属于web指纹。


## Web指纹的分类


Web指纹可以根据不同的应用分成不同的类型，如下表所示：
 
指纹分类<br>
示例<br>
Web容器<br>
Apache、Nginx、IIS、Tomcat、Weblogic<br>
Web容器模块<br>
Squid、OpenSSL、mod_dav<br>
Web服务端语言<br>
PHP、Java、.NET、Nodejs<br>
Web后端框架<br>
Thinkphp、Struts2<br>
Web应用<br>
Wordpress、seacms<br>
Web前端框架<br>
Vue、angularjs、react、Highcharts<br>
Web前端语言<br>
Javascript、less<br>
Web运营商<br>
移动、联通<br>
第三方内容<br>
YouTube<br>
Cdn运营商<br>
阿里云，电信<br>
组织机构<br>
BACKBONE No.31,Jin-rong Street<br>
ISP服务商<br>
CHINANET-BACKBONE No.31,Jin-rong Street<br>
网站类型<br>
政府网站、企业门户、个人博客<br>
操作系统<br>

## Web指纹的识别方式

指纹识别的技术其实也还是众所周知的几个识别方向：<br>

1.header判断

2.body关键词匹配

3.url内容的md5匹配

4.url状态码判断

5.url相对路径匹配

## 功能介绍
wmap是一款用于对远程web应用进行快速指纹探测的引擎，采用异步io+协程的网络处理方式。<br>
- 支持指定并发线程数和服务器的最大并发连接数
- 采用keepalive的方式，减少http短连接的频繁释放
- 支持dns缓存
- 采用插件化开发，可以定制信息类或漏洞检测类插件。
- 采用json规则方式对Web指纹进行识别
- 支持100多种cms的类型和版本识别，支持50多种Web服务器及版本的识别