# 关于loading

使用CSS3模仿win10的loading效果。

## 如何使用

使用loading你需要下面两个步骤：
1. 将loading的HTML代码放到您的HTML中。
2. 加载loading的css样式。

## 如何修改loading的样式

loading可以让你定制：
* 旋转的直径（当然，指的是旋转边界的半径。例如：您设置直径为100px，那么loading会在100px内旋转，而不是旋转点是100px的直径。一般旋转点的直径大致为直径的60%）
* 旋转点的直径，这个是真直径。
* loading旋转一圈的时间，单位为s
* 旋转点的颜色。

方法：

1. 打开`src/loading.less`文件。
2. 看最后一行`.loading-panel(60px, 4px, 1.4s, #c03);`。参数分别代表：旋转直径，旋转点直径，旋转周期时间和旋转点颜色。修改成你需要的。
3. 打开cmd或其他终端工具，在项目目录下执行：`lessc .\src\loading.less > .\src\loading.css`。
4. 刷新项目目录下的example.html查看效果。

## 代码说明

你可在`/src`中查看Loading的源代码。less文件为源码，css为LESS生成的。如要修改，请自行修改less文件。

在你使用loading的时候，可以减少或增加旋转点的个数，
`<div class="point"><div class="inner"></div></div>`的个数越多，旋转点就越多。**loading最多支持10个旋转点**
