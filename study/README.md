## CSS

### 外部是如何引入的？

1.css是通过`link`标签引入到html里面的

~~~html
<head>
<link rel="stylesheet" href="./(CSS的目标地址)">
</head>
~~~

2.在<head>标签里引入<style>标签,并在<style>标签里写CSS

~~~html
<head>
<style>
 /* CSS代码 */
</style>
</head>
~~~

3.在标签内的style属性里面直接书写CSS

~~~html
<标签名 style="property:value;">
~~~



### 在CSS的标准盒模型当中，元素的总宽度?

边框盒宽=width

内容盒宽= width - padding - border

实际占用宽= width + margin

**总宽度** = width + padding-left + padding-right + border-left + border-right + margin-left + margin-right



###  CSS的什么伪类用于选择鼠标悬停时的元素状态？

:hover伪类选择器

~~~html
    <style>
        /* 伪类选择器用：hover */
        a:hover {
            color: red;
        }
        div:hover {
            color: green;
        }
    </style>
~~~



### CSS选择器的优先级按顺序从高到低为？

1. **style属性**
2. **ID选择器**
3. **类选择器/属性选择器/伪类选择器**
4. **元素/伪元素选择器**



### 在CSS中，使用什么可以使某个样式规则具有更高的优先级，覆盖普通规则？

`!important`声明