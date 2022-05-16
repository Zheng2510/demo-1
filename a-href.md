# a的href属性

## 英语课
* 英语 翻译 助记 英语 翻译 助记 
* hyper 超级 (害怕) blank 空白
* target 目标 (他给他) parent 父母之一 (盼望他)
* reference 引用 (refer+ence) self 自己
* frame 边框,框架 load 加载
* error 错误 (哎惹) canvas 画布
## a标签
### 常用属性
* href(两个单词缩写hyper+reference超级引用/链接)
* target 指定在哪个窗口打开超链接 
* download 下载网页而不是查看网页
* rel=noopener(面试可能会问)

## 不要双击打开html 
### 方法一使用http server 打开
1. 打开终端安装 yarn global add http-server
2. 步骤打开终端运行http-server . -c-1(-c是缓存-1是不要缓存) 
3. ctrl+单机打开,后缀加上文件名
### 方法二
1. 打开终端安装yarn global add parcel
2. 步骤终端运行parcel 加上文件名 
3. ctrl+单机打开
### a的href的取值
* 网址(手机访问在同一个wifi下)
1. https://google.com (以https为开头的网址)
2. http://google.com (以htto为开头的网址)
3. //google.com (以//为开头的网址,无协议的网址)运行后,ctrl+单机打开页面后,注意先右击打开开发者工具-点击network(网络)-勾选preservelog(保留日志)-再点击链接 
* 路径
1. /a/b/c以及a/b/c(在哪里开的服务,那里就是根目录,所以双击直接打开会直接从硬盘开始 )
代码
```javascript
 <a href="/a/b/c.html">c.html</a>
 <a href="a/b/c.html">c.html</a>
```


2. index.html以及./index.html(可以直接用index.html)
代码
```javascript
<a href="index.html">c.html</a>
<a href="./index.html">c.html</a>
```
* 伪协议
1. javascript:代码;
下面是代码
```javascript
<a href="javascript:alert(1);">JavaScript伪协议</a>
  <a href="javascript:;">空的伪协议</a>
```
* href内容为空,点击链接刷新页面,而输入javascript:;,是什么都不做的查看

1. mailto:邮箱
   下面是代码
```javascript
  <a href="mailto:1741167304@qq.com">发邮件</a>
```
3. tel:手机号
下面是代码
```javascript
 <a href="tel:13105352510">打电话</a>
```
4. href加指定id的作用,跳转到指定标签
```
href=#xxx
```

### a标签的作用
* 跳转到外部页面
* 跳转到内部锚点
* 跳转到邮箱或者电话等
