# ProgressBar
常见的网页进度条加载

### 或许有用的网站
1、[免费的gif动画下载](https://icons8.com/preloaders);<br>
2、[另外一个免费的gif动画下载](https://loading.io/);<br>
3、[自动处理CSS 3前缀在线网站](http://autoprefixer.github.io),代码粘贴进去，等待一段时间即可。<br>

### Demo1定时的进度条
这是一个伪加载完成的进度条，页面跳转时间由自己来设置，实用性并不高。<br>
[案例演示](https://cruxf.github.io/ProgressBar/Demo1.html)

### Demo2通过加载状态触发的进度条
知识点：<br>
1、document.onreadystatechange  页面加载状态改变时的事件<br>
2、document.readyState  返回当前文档的状态<br>
相关readyState状态码：<br>
1、uninitialized  还未开始载入<br>
2、loading  载入中<br>
3、interactive  已加载，文档与用户可以开始交互<br>
4、complete  载入完成<br><br>
通过对页面的加载状态来触发相应的事件，这是一种合适的进度条制作。<br>
[案例演示](https://cruxf.github.io/ProgressBar/Demo2.html)

### Demo3通过CSS3制作进度条
利用CSS3动画制作的进度条效果，简单好玩，同样也是通过加载状态来触发相应的事件。<br>
[案例演示](https://cruxf.github.io/ProgressBar/Demo3.html)

### Demo4固定在头部的进度条
在每一段结构代码后面添加jQuery中的animate方法增加固定在顶部元素的长度，当长度达100%后触发事件，隐藏遮罩层，这也是一种伪加载完毕事件，实用性并不强。<br>
[案例演示](https://cruxf.github.io/ProgressBar/Demo4.html)

### Demo5实时监测加载的进度条
知识点：<br>
1、建立图像对象：var 名称 = new Image()<br>
2、属性：border complete height...<br>
3、事件：onload onerror onkeydown onkeypress...<br>
4、src属性一定要写到onload的后面，否则程序在IE中会出错<br>
用户体验比较好的一种加载方式，能够随时随地知道资源加载到了哪一步。<br>
[案例演示](https://cruxf.github.io/ProgressBar/Demo5.html)
