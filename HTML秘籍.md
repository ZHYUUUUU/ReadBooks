HTML秘籍/进度P11
###  阅读笔记：

> 在编写html时， 引用本地javascript时，时不时弹出“为帮助保护您的安全，Internet Explorer 已经限制此文件显示可能访问您计算机的活动内容。单击此处查看选项…” 框。 

解决办法只需要在引用javascript前添加注释语句 ```<!-- saved from url=(0014)about:internet --> ```。 但是格式空格要注意下：在```<!--与saved单词间只空一格空格，后面的internet单词与 -->```间至少空一格空格，推荐只空一格。否则还是会弹出来。 

``` HTML  
<!DOCTYPE HTML>  
<html>  
<head>  
<title>Examole html page</title>  
<meta charset="utf-8" />  
<!-- saved from url=(0014)about:internet -->  
<script>document.write('hello world');</script>  
</head>  
<body>  
<!--内容此处-->  
</body>  
</html>  
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTI2NTI2ODk2XX0=
-->