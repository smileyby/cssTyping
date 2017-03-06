CSS实现打字效果
=============

#### 主要代码如下：

```html

	<!DOCTYPE html>
	<html lang="en">
	<head>
	  <meta charset="UTF-8">
	  <title>CSS实现打字效果</title>
	  <style type="text/css">
		@keyframes typing {
		    from {
		        width:0;
		    }
		}
		@keyframes blink-caret {
		    50% {
		        border-color:transparent;
		    }
		}
		h1 {
		    font:bold 200% Consolas,Monaco,monospace;
		    border-right:.1em solid;
		    width:6.6em;
		    margin:2em 1em;
		    white-space:nowrap;
		    overflow:hidden;
		    animation:typing 2s steps(12,end),blink-caret .5s step-end infinite alternate;
		}
	  </style>
	</head>
	<body>
		<h1>Hello World!</h1>
	</body>
	</html>

```

[MDN关于animation属性的用法](https://developer.mozilla.org/zh-CN/docs/Web/CSS/animation)