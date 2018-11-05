# CSS3
## 边框
```
div
{
border:2px solid;
border-radius:25px; // 圆角边框
-moz-border-radius:25px; /* Old Firefox */
box-shadow: 10px 10px 5px #888888; 边框阴影

div
{  // 边框图片
border-image:url(border.png) 30 30 round;
-moz-border-image:url(border.png) 30 30 round; /* 老的 Firefox */
-webkit-border-image:url(border.png) 30 30 round; /* Safari 和 Chrome */
-o-border-image:url(border.png) 30 30 round; /* Opera */
}
}
```
## 背景
> 新的背景属性
```
background-clip	规定背景的绘制区域。
background-origin	规定背景图片的定位区域。
background-size	规定背景图片的尺寸。
```
> 多重背景图片
```
body
{
background-image:url(bg_flower.gif),url(bg_flower_2.gif);
}
```
## 文本效果
> 新的文本属性
```
hanging-punctuation	规定标点字符是否位于线框之外。
punctuation-trim	规定是否对标点字符进行修剪。
text-align-last	设置如何对齐最后一行或紧挨着强制换行符之前的行。
text-emphasis	向元素的文本应用重点标记以及重点标记的前景色。
text-justify	规定当 text-align 设置为 "justify" 时所使用的对齐方法。
text-outline	规定文本的轮廓。
text-overflow	规定当文本溢出包含元素时发生的事情。	3
text-shadow	向文本添加阴影。
text-wrap	规定文本的换行规则。
word-break	规定非中日韩文本的换行规则。
word-wrap	允许对长的不可分割的单词进行分割并换行到下一行。
```
> 单词自动换行
```
p {word-wrap:break-word;}
```
> 文字阴影
```
h1{text-shadow: 5px 5px 5px #FF0000;}
```
## 字体
```
<style>
@font-face
{
font-family: myFirstFont;
src: url('Sansation_Light.ttf'),
     url('Sansation_Light.eot'); /* IE9+ */
}

div
{
font-family:myFirstFont;
}
</style>
```
## 2D转换
> rotate
```
div
{
transform: rotate(30deg);
-ms-transform: rotate(30deg);		/* IE 9 */
-webkit-transform: rotate(30deg);	/* Safari and Chrome */
-o-transform: rotate(30deg);		/* Opera */
-moz-transform: rotate(30deg);		/* Firefox */
}
```
> translate
```
div
{
transform: translate(50px,100px);
-ms-transform: translate(50px,100px);		/* IE 9 */
-webkit-transform: translate(50px,100px);	/* Safari and Chrome */
-o-transform: translate(50px,100px);		/* Opera */
-moz-transform: translate(50px,100px);		/* Firefox */
}
```
> scale
```
div
{
transform: scale(2,4);
-ms-transform: scale(2,4);	/* IE 9 */
-webkit-transform: scale(2,4);	/* Safari 和 Chrome */
-o-transform: scale(2,4);	/* Opera */
-moz-transform: scale(2,4);	/* Firefox */
}
```
## 3D转换
> rotateX()  x轴旋转
```
div
{
transform: rotateX(120deg);
-webkit-transform: rotateX(120deg);	/* Safari 和 Chrome */
-moz-transform: rotateX(120deg);	/* Firefox */
}
```
> 通过 rotateX() 方法，元素围绕其 X 轴以给定的度数进行旋转
```
div
{
transform: rotateY(130deg);
-webkit-transform: rotateY(130deg);	/* Safari 和 Chrome */
-moz-transform: rotateY(130deg);	/* Firefox */
}
```
## 过渡
```
div
{
transition: width 1s linear 2s;
/* Firefox 4 */
-moz-transition:width 1s linear 2s;
/* Safari and Chrome */
-webkit-transition:width 1s linear 2s;
/* Opera */
-o-transition:width 1s linear 2s;
}
```
## 动画
> CSS3 @keyframes 规则
```
@keyframes myfirst
{
from {background: red;}
to {background: yellow;}
}

@-moz-keyframes myfirst /* Firefox */
{
from {background: red;}
to {background: yellow;}
}

@-webkit-keyframes myfirst /* Safari 和 Chrome */
{
from {background: red;}
to {background: yellow;}
}

@-o-keyframes myfirst /* Opera */
{
from {background: red;}
to {background: yellow;}
}
```
## 多列
```
div
{
-moz-column-count:3; 	/* Firefox */
-webkit-column-count:3; /* Safari 和 Chrome */
column-count:3;
}
```
> 新的多列属性
```
column-count	规定元素应该被分隔的列数。
column-fill	规定如何填充列。
column-gap	规定列之间的间隔。
column-rule	设置所有 column-rule-* 属性的简写属性。
column-rule-color	规定列之间规则的颜色。
column-rule-style	规定列之间规则的样式。
column-rule-width	规定列之间规则的宽度。
column-span	规定元素应该横跨的列数。
column-width	规定列的宽度。
columns	规定设置 column-width 和 column-count 的简写属性
```
## 用户界面
> 新的用户界面属性
```
appearance	允许您将元素设置为标准用户界面元素的外观
box-sizing	允许您以确切的方式定义适应某个区域的具体内容。
icon	为创作者提供使用图标化等价物来设置元素样式的能力。
nav-down	规定在使用 arrow-down 导航键时向何处导航。
nav-index	设置元素的 tab 键控制次序。
nav-left	规定在使用 arrow-left 导航键时向何处导航。
nav-right	规定在使用 arrow-right 导航键时向何处导航。
nav-up	规定在使用 arrow-up 导航键时向何处导航。
outline-offset	对轮廓进行偏移，并在超出边框边缘的位置绘制轮廓。
resize	规定是否可由用户对元素的尺寸进行调整。
```