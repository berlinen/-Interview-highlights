---
title: 'css值和单位'
---

<Block>
# css值和单位
</Block>

<Block>
## 你有没有使用过视网膜分辨率的图形？当中使用什么技术？

所谓“Retina”是一种显示标准，是把更多的像素点压缩至一块屏幕里，从而达到更高的分辨率并提高屏幕显示的细腻程度。

</Block>

<Block>
##  px，em，rem，vw 有什么区别？

### px

px就是pixel的缩写，意为像素。px就是一张图片最小的一个点，一张位图就是千千万万的这样的点构成的，比如常常听到的电脑像素是1024x768的，表示的是水平方向是1024个像素点，垂直方向是768个像素点。

### em
参考物是父元素的font-size，具有继承的特点。如果自身定义了font-size按自身来计算（浏览器默认字体是16px），整个页面内1em不是一个固定的值。

### rem
css3新单位，
相对于根元素html（网页）的font-size，不会像em那样，依赖于父元素的字体大小，而造成混乱。

### %
一般宽泛的讲是相对于父元素，但是并不是十分准确。
1、对于普通定位元素就是我们理解的父元素

2、对于position: absolute;的元素是相对于已定位的父元素

3、对于position: fixed;的元素是相对于 ViewPort（可视窗口）

### vwcss3新单位
viewpoint width的缩写，视窗宽度，1vw等于视窗宽度的1%。举个例子：浏览器宽度1200px, 1 vw = 1200px/100 = 12 px。

### vhcss3新单位
viewpoint height的缩写，视窗高度，1vh等于视窗高度的1%。举个例子：浏览器高度900px, 1 vh = 900px/100 = 9 px。

### vmcss3新单位
相对于视口的宽度或高度中较小的那个。其中最小的那个被均分为100单位的vm

### 介绍下 BFC 及其应用。

BFC是CSS布局的一个概念，是一块独立的渲染区域，是一个环境，里面的元素不会影响到外部的元素 。

#### 如何生成BFC：（即脱离文档流）

1、根元素，即HTML元素（最大的一个BFC）
2、float的值不为none
3、position的值为absolute或fixed
4、overflow的值不为visible（默认值。内容不会被修剪，会呈现在元素框之外）
5、display的值为inline-block、table-cell、table-caption

#### BFC布局规则：

1.内部的Box会在垂直方向，一个接一个地放置。


2.属于同一个BFC的两个相邻的Box的margin会发生重叠


3.BFC就是页面上的一个隔离的独立容器，容器里面的子元素不会影响到外面的元素。反之也如此, 文字环绕效果，设置float


4.BFC的区域不会与float box重叠。


5.计算BFC的高度，浮动元素也参与计算

#### BFC作用：

1.自适应两栏布局

2.可以阻止元素被浮动元素覆盖

3.可以包含浮动元素---清除内部浮动 原理：触发父div的BFC属性，使下面的子div都处在父div的同一个BFC区域之内

4.分属于不同的BFC时，可以阻止margin重叠

</Block>

