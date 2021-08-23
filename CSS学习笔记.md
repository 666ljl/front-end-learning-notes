# 前端三大基础
- HTML（结构）
- **CSS（表现）**
- Javascript（行为）
嗯嗯嗯

# 一、CSS（Cascading Style Sheets）
- CSS 描述了如何在屏幕、纸张或其他媒体上显示 HTML 元素
- CSS 节省了大量工作，它可以同时控制多张网页的布局
- 外部样式表存储在 CSS 文件中



# 二、CSS语法
选择器+声明块

![avatar](https://www.w3school.com.cn/i/css/selector.gif)

- 选择器：指向需要设置样式的 HTML 元素
- 声明块：包含一条或多条用分号分隔的声明。每条声明都包含一个 CSS 属性名称和一个值，以冒号分隔

## css放置位置
- 1、内部
```html
<html>
<head>
    <titile></title>
    <style type="text/css">
        //在这里写CSS代码
    </style>
</head>
<body>
</body>
</html>
```
- 2、行内
 ```html
<html>
<head>
    <titile></title>
</head>
<body>
    <div style="width="100px" height="100px""></div>
</body>
</html>
```
- 3、外部
```html
<html>
<head>
    <titile></title>
    <link rel="stylesheet" href="要引入的CSS文档位置.css" >
</head>
<body>
</body>
</html>
```

# 三、选择器
## 1.元素选择器
元素选择器根据元素名称来选择HTML元素
```html
p {
  text-align: center;
  color: red;
}
```
## 2.id选择器
id选择器使用HTML元素的id属性来选择特定元素。
```html
#para1 {
  text-align: center;
  color: red;
}
<p id=para1>。。。</p>
```
## 3.类选择器
.center {
  text-align: center;
  color: red;
}
或者
h1.center
```html
<h1 class="center">居中的红色标题</h1>
<p class="center">居中的红色段落。</p> 
```

## 4.通用选择器
通用选择器（*）选择页面上的所有的 HTML 元素。
```html
* {
  text-align: center;
  color: blue;
}
```

## 5.分组选择器
分组选择器选取所有具有相同样式定义的 HTML 元素。
```html
h1, h2, p {
  text-align: center;
  color: red;
}
```

## 6.属性选择器
```html
*[title] {color:red;}
```
```html
a[href] {color:red;}
或者
a[href][title] {color:red;}
```
## 7.后代选择器
后代选择器（descendant selector）又称为包含选择器。
```html
h1 em {color:red;}
```

## 8.子元素选择器
子元素选择器（Child selectors）只能选择作为某元素子元素的元素。
```html
h1 > strong {color:red;}
```
# 四、颜色
```html
style="color:Tomato;" 文本颜色
style="border:2px solid Tomato;" 边框
style="background-color:rgb(255, 99, 71);" 背景
```
# 五、图像
```html
background-color
background-image：url()
```
# 六、边框
border-style
border-width

# 七、边距
margin:用于控制元素与元素之间的距离

padding:用于控制内容与边框之间的距离

![avatar](https://www.w3school.com.cn/i/css/boxmodel.gif)

# 八、字体
## 1.字体分类
- 衬线字体（Serif）：在每个字母的边缘都有一个小的笔触。它们营造出一种形式感和优雅感。
- 无衬线字体（Sans-serif）：字体线条简洁（没有小笔画）。它们营造出现代而简约的外观。
- 等宽字体（Monospace）：这里所有字母都有相同的固定宽度。它们创造出机械式的外观。
- 草书字体（Cursive）：模仿了人类的笔迹。
- 幻想字体（Fantasy）：是装饰性/俏皮的字体。

## 2.字体属性
- font-style
- font-variant
- font-weight
- font-size/line-height
- font-family

# 九、链接
- a:link  正常的，未访问的链接
- a:visited  用户访问过的链接
- a:hover  用户将鼠标悬停在链接上时
- a:active  链接被点击时

# 十、表格
table  tr th
