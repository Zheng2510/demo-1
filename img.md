# img标签
```javascript
 <img src="" alt="">
```
* src-source(后面接的内容一般是图片的地址,可以是网络地址也可以是相对路径或者绝对路径)
### 作用
* 发出get请求,展示一张图片
* get请求查看方法,打开开发者工具,选择network-在名称右键把method打开
### 属性
* alt/height/width/src
1. alt 在图片加载失败时候,显示一个字来提示用户
2. height,width高和宽-只支持像素,如果只写高度,宽度会自适应(注意:永远不能让图片变形)
### 事件
* onload/onerror(用来监听图片是否加载成功了)
* 成功调用onload不成功onerror
### 响应式
* max-width:100%(响应式,不会固定宽度)
```javascript
<style>
        img {
            max-width: 100%;
        }
    </style>
```
### 可替换元素(考试可能会问)