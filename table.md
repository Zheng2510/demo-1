# table标签
### table里面只能有三个标签
```javascript
 <thead></thead>
 <tbody></tbody>
 <tfoot></tfoot>
```
* thead 头部
* tr -table row (table里面的一行) 
* th-表示一个表头
* td-table data 数据
### 当你写的table里面没有thead，tbody，tfoot的时候，里面写的tr的内容会默认放在tbody里，如果只写td，那么会默认加上tbody和tr
### 相关样式
1. table-layout
* auto-大多数用，表格及单元格的宽度取决于其包含内容
```javascript
<style>
    table {table-layout: auto;
           width: 600px;}
    </style>
```
* fixed-表格和列的宽度通过表格的宽度来设置
```javascript
  <style>
    table {table-layout: fixed;
           width: 600px;}
    </style>
```
1. border-collapse(用来注意border是否合并，collapse意思是合并)
```javascript
    <style>
    table {table-layout: fixed;
           width: 600px;
        border-collapse: collapse;
        border-spacing: 0px;}
        td,th{
            border: 1px solid blue;
        }
    </style>
```

2. border-spacing(控制表格之间的距离)