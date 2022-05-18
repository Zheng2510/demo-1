# form标签
## 作用
* 发出get或post请求,然后刷新页面
## 属性
* action/autocomplete(自动填充)/method(方法)/target
1. action里面写什么,点击之后就会请求到哪个页面
2. method 控制用get还是post
3. autocomplete
下面是代码
```javascript
 <form action="/xxx" method="post" autocomplete="on" target="_blank">
        <input name="username" type="text"/>
        <input type="submit" />
```
* 在form里加autocomplete,在input加name,只要在输入的地方就会给出自动的建议
* target-提交到哪个页面,哪个页面就刷新
## 事件
* onsubmit

* input和button区别-input不支持其他标签button支持
```javascript
 <input type="submit" value="搞起" />
    <button type="submit">
        <strong>搞起</strong>
    </button>
```
* form必须要有一个type="submit"那么这个表单才可以提交
## input标签
### 作用
* 让用户输入内容
### 属性
* 类型type:
1. button
2. checkbox(多选)
* 如何让多选是一组,加上同一个name
```
<input type="checkbox" name="hobby"/>唱
<input type="checkbox" name="hobby"/>跳
<input type="checkbox" name="hobby"/>rap
<input type="checkbox" name="hobby"/>篮球
```
3. email
4. file(上传头像,文件)
* 默认只能选择一个文件,选择多个文件需要加上multiple
```
<input type="file"/>
<input type="file" multiple/>
```
5. hidden(看不见的,是给机器输入的)
```
看不见hidden<input type="hidden"/>
```
6. number
7. password(不展示具体内容;密码)
```
<input type="password"/>
```
8. radio(单选)如果想二选一就让它们有一个共同的name
一般用gender表示性别
```
<input name="gender" type="radio"/>男
<input name="gender" type="radio"/>女
```
9.  search
10.  submit
11.  tel
12.  text(默认,文本)
```
 <input type="text"/>
```
13. color(颜色)
```
  <input type="color"/>
```
14. testarea(多行文本输入)
* 默认右下角可以拖拽,加上style="resize:none,可以固定
```
<textarea style="resize:none;width: 50px;height: 100px;"></textarea>
```
15. select(选择)
```
<option value="">-请选择-</option>
<option value="1">星期一</option>
<option value="2">星期二</option>
```
* 其他:
1. name
2. autofocus
3. checked
4. disabled
5. maxlength
6. pattern
7. value
8. placeholder
### 事件
1. onchange(当用户输入改变的时候触发onchange)
2. onfocus
3. onblur
### 验证器
* HTML5新增功能

### 注意事项
1. 一般不监听input的click事件
2. form里面的input要有name
3. form里面放一个type=submit才能触发submit事件

### 其他标签
* video
* audio
* canvas
* svg

### 注意事项
* 这些标签的兼容性一定要查看文档

