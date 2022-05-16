# a的target的取值
### 内置
* _blank (在空白页面打开)
```javascript
<a href="htttps://google.com" target="_blank">google</a>
```
* _top(打开最顶端窗口)
```javascript
<a href="https://google.com" target="_top">google</a>
    <div>
        <iframe src="a-target-iframe.html" frameborder="0"></iframe>
    </div>
```
* _parent(在当前链接所在的上一层打开)
* _self(在当前页面打开-默认值)
```javascript
 <a href="https://google.com" target="_self">google</a>
 ```
* target = "xxx"(如果有一个叫xxx的窗口就用它,如果没有就创建一个,把它叫做xxx.这个xxx就是这个新窗口的名字)
```javascript
<a href="https://google.com" target="xxx">google</a>
<a href="https://baidu.com" target="xxx">baidu</a>
```
## 程序员命名
* window的name(右击打开开发者工具-控制台-输入window.name查看名字)
如何命名
```javascript
<a href="https://google.com" target="xxx">google</a>
<a href="https://baidu.com" target="xxx">baidu</a>
```
* iframe的name
```javascript
  <a href="https://google.com" target="xxx">google</a>
    <a href="https://baidu.com" target="yyy">baidu</a>
    <hr>
    <iframe src="" name="xxx" frameborder="0">xxx</iframe>
    <hr>
    <iframe src="" name="yyy" frameborder="0">yyy</iframe>
```