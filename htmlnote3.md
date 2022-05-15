# html笔记三

## vscode插件推荐
* prettier 更好的格式化工具
  
## jsbin 代码编辑器(缺点单文件只能编辑一个文件的)
## 代码沙盒 codesandbox.io  (加图片只有拖动图片进去一个方法)

## 章节标签
### 表示文章/书的层级
* 标题h1~h6
* 章节section
* 文章article
* 段落p
* 头部header
* 脚部footer
* 主要内容main
* 旁支内容aside
* 划分div
下面是我的代码
```
 <!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <title>JS Bin</title>
</head>

<body>
  <header>顶部广告</header>
  <div>
    <main>
      <h1>文章标题</h1>
      <h2>副标题</h2>

      <section>

        <h2>第一章</h2>
        <p>
          我大把大把发布第三部分是大部分克里斯蒂
        </p>

        <section>
          <h3>第二章</h3>

          <p>
            这是一段话
          </p>
        </section>
      </section>
    </main>
    <aside>
      参考资料导航
    </aside>
  </div>
  <footer>&copy.版权所有</footer>
</body>

</html>
``` 
## 全局属性
### 所有标签都有的属性
* class
* contenteditable(可以使任何一个元素被编辑可编辑的)
* hidden(让一个属性看不见)
* id(全页面唯一用id 不到万不得已不要用id因为id不报错,用法是可以加名字,js可以直接调用id)
* style(如果把style放在body里 用style{display:block;}可以使style标签显示 可以让用户自己修改样式)
* tabinex(控制顺序,0是最后一个,-1表述不妨问我)
* title(用来显示完整内容)
style css js属性同时存在的话优先级js 

## 默认样式
### 为什么有默认样式
* 因为发明HTML的时候,css还没出生
### 怎么看默认样式
* chrome开发者工具
* Elements->Styles->user agent stylesheet
### user agent
* 就是浏览器
### css reset
默认样式不符合我们的需求
### 常见样式可以抄大厂代码
* 进入大厂首页
* Chrome开发者工具,找到类似代码
* 复制到自己项目
* 命名为reset.css
* 方方老师常用{地址}(https://gist.github.com/FrankFang/df5e57a0799823ed89a960a642b3a1e2)
  下面是代码
```javascript

  * {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
*::before,
*::after {
  box-sizing: border-box;
}
a {
  color: inherit;
  text-decoration: none;
}
input,
button {
  font-family: inherit;
}
ol,
ul {
  list-style: none;
}
table {
  border-collapse: collapse;
  border-spacing: 0;
}

```

## 常用内容标签
* ol+li   (ol全称 ordered list 有顺序的列表 li全称list item列表中的一项)
* ul+li   (ul全称 unordered list 无顺序的列表)
* dl+dt+dd (dl全称 description list 描述列表  t全称term表示概念被描述的词 dd全称data)
* pre(保留空格回车和tab)
* hr--分割线
* br--全称break 中断打断(回车)
* a--超链接
* em--表示强调(语气)
* strong--本身很重要的强调
* code(里面的字体等宽,方便写代码)
* quote(行内的引用)
* blockquote(块级的引用)