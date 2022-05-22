# 小网页
### 添加图片
* 注意不要让图片变形
* 如果图片比例不对,需要使用工具裁剪
* 如果图片尺寸过大,无需特殊处理
* 如果图片体积过大(300kb),则需压缩

### 添加链接
* 国内一般需要添加 target=_blank
* 添加完了之后要全部点一遍,防止出错

## 怎么兼容手机
1. meta:vp完整版(补全)
```javascript
    <meta name="viewport" content="width=device-width, initial-scale=1.0,minimum-scale=1.0, maximum-scale=1.0, user-scalable=no">
```
2. img{
         max-width:100%; 
     }

## 1用wifi调试手机
### 步骤
1. 让手机和电脑处于同一个wifi
2. 手机可以直接用IP和端口访问电脑
3. 用哪个IP?http-server给出的ip全部试一遍
4. 用border调试法调试css
5. 用vconsole.js调试js
## 2用chrome远程调试
### 步骤
* 搜索chrome远程调试
* 按照教程 {网址}[https://developer.chrome.com/docs/devtools/remote-debugging/]
* 按照视频配置一下

## 将网址部署到GitHub pages
* 步骤-创建本地仓库-提交代码-上传到github-选择settings-选择github pages-选择分支保存
* 将地址复制-返回仓库-选择edit-粘贴地址
### 免费的服务器
* 注意用户体验
* 细节决定成败
* 把预览地址放在显眼的地方
