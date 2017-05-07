# jquery

使用jquery编写的代码:
```
$(document).ready(function(){
    //程序段
})
```
使用传统javascript编写的代码:
```
window.onload = function(){
    //程序段
}
```
虽然上述两段代码在动能上可以互换,但是它们之间又有许多区别:
* 执行时间不同: $(document).ready()在页面框架下载完毕后就执行:而window.onload必须在页面全部加在完毕(包含图片下载)后才能执行.很明显,前者的执行效率高于后者
* 执行数量不同: $(document).ready()可以重复写多个,并且每次执行结果不同,而window.onload尽管可以执行多个,但是仅输出最后一个执行结果,无法完成多个结果的输出
* $(document).ready(function(){})可以简写成$(function(){})
