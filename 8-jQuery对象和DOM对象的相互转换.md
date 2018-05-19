### jQuery对象和DOM对象的互相转换
	
#### jQuery对象转换成DOM对象

1. 方式一

		$("#btn")[0]

2. 方式二

		$("#btn").get(0)

#### DOM对象转换成jQeury对象

1. 方式一

		$(document): 将DOM对象转换成jQuery对象
		
2. 方式二

		1. 先通过原生JS获取到元素对象
		var btn = document.getElementById("btn");
		2. 再转换成jQuery对象
		$(btn)