### $问题

1. JS命名语法: 

		下划线, 字母, $, 数字, 但是不能以数字开头
		var $ = "我是$符号";

jQuery占用 $ 和 jQuery 两个变量

### JS和jQuery入口函数的区别

1. JS的window.onlaod事件是等到所有的内容, 包括外部图片之类的文件加载完成之后, 才去执行
2. jQuery的入口函数, 是在HTML所有标签都加载后, 回去执行

### JS创建对象

三种方式:

1. 方式一
		
		var obj = {};
2. 方式二

		var obj = new Object();
3. 方式三

		var obj = Object.create();

方式一和方式二的区别: 

1. 推荐使用方式一
2. 方式二存在效率问题, new对象, 涉及到原型查找问题


	
