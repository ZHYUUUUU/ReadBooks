## HTML5秘籍
<kbd>阅读笔记</kbd> <kbd>进度:P11/P360 </kbd>

### 1. 在编写html时， 引用本地javascript时，时不时弹出“为帮助保护您的安全，Internet Explorer 已经限制此文件显示可能访问您计算机的活动内容。单击此处查看选项…” 框。

解决办法只需要在引用javascript前添加注释语句 ```<!-- saved from url=(0014)about:internet --> ```。 但是格式空格要注意下：在```<!--与saved单词间只空一格空格，后面的internet单词与 -->```间至少空一格空格，推荐只空一格。否则还是会弹出来。

``` HTML
<!DOCTYPE HTML>
<html lang="en">
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

#### 2. HTML5新增元素
用于构建页面的语义元素：
```<article>、<aside>、<figcaption>、<figure>、<footer>、<header>、<hgroup>、<nav>、<secton>、<details>、<summary>```
用于标识文本的语义元素：
```<mark>、<time>、<wbt>(以前就支持，但现在正式列入规范)```
Web表单及交互：
```<input>(不是新元素，但增加了很多类型)、<datalist>、<keygen>、<meter>、<progress>、<command>、<menu>、<output>```

<!--stackedit_data:
eyJoaXN0b3J5IjpbNTI3Mzc2MDAzLDU4ODA0MzU1OSwxNDk3ND
E2NjQyLC0zMTc4OTAwNjUsMTc5NDg0Njg5OSwtMzczMzkxMDg5
LC0xMTE0NjgyOTU3XX0=
-->