### 1. jQuery的作用

jQuery是基于JavaScript的一个库, 对常用功能进行封装, 包含多个可重用的函数, 用于辅助简化JavaScript的开发, 提高开发效率

用于解决原生JavaScript使用的一些问题:

1. window.onload事件覆盖的问题
2. 代码容错性差
3. 浏览器兼容性问题
4. 书写繁琐, 代码量多
5. 代码很乱
6. 动画效果实现难

### 2. jQuery的基本使用

#### 2.1 引包

1. 下载jQuery源文件, 并放到项目中
2. 在页面中引入jQuery文件
		<script src="jquery-版本号.min.js"></script>

#### 2.2 入口函数

1. 方式一

		$(document).ready(function(){

		});

2. 方式二

		$(function(){

		});

3. jQuery入口函数的伪代码实现

		var iQuery = function(dom){
			var obj = function(){
				ready : function(func){
					//func();
					//判断 document.onload有没有被赋值(有没有onlaod事件)
					//有: 接收旧的函数, 然后先去调用新的函数, 接着在调用旧的函数
					//没有: 直接赋值给onload事件
					if(typeof dom.onlaod === "function"){
						var oldFunc = dom.onload;
						dom.onload = function(){
							//调用新的函数
							func();
							//调用旧的函数
							oldFunc();
						}
					}else{
						dom.onload = func;
					}
				}
			}
		};

		iQuery(window).ready(function(){
			console.log("我是function");
		});

4. jQuery和JS的入口函数的区别:

	 	1. JS的window.onlaod事件是等到所有的内容, 包括外部图片之类的文件加载完成之后, 才去执行

		2. jQuery的入口函数, 是在HTML所有标签都加载后, 回去执行


#### 2.3 事件处理程序

1.事件源

	JS的方式: document.getElementById("id");
	jQuery方式: $("#id")

2.事件

	JS的方式: document.getElementById("id").onclick
	jQuery方式: $("#id").click

***区别: jQuery的事件不带on***

3.事件处理程序
	
	JS的方式:
	document.getElementById("id").onclick=function(){

	}

	jQuery的方式:
	$("#id").click(function(){

	});

