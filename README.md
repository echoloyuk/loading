# 关于Loading

使用CSS3模仿win10的loading效果，虽然还没有100%还原，但是已经基本实现效果。

# 如何使用

请使用支持CSS3的浏览器打开example.html，页面正中央会出现Loading效果。

# 代码说明

您可在`/src`中查看Loading的源代码。less文件为源码，css为LESS生成的。如要修改，请自行修改less文件。

在less文件中，只有最后一行是真正less实现。`.loading-panel(60px, 4px, 1.4s);`中60px为loading的边框的宽高；4px位原点半径，1.4s为单个原点旋转一周的时间。

请修改后重新执行less

````
lessc ./src/loading.less > ./src/loading.css
````
