### jQuery基本选择器

#### 1. CSS选择器

1. id选择器

		符号: #id
		用法: 
			#id { color: red; }

2. 类选择器

		符号: .class
		用法: 
			.class { color: red; }

3. 标签选择器

		符号: Element
		用法: 
			p { color: red; }

4. 通配符选择器

		符号: *
		用法: 
			* { color: red; }
			
		一般配合其他选择器进行使用

5. 后代选择器

		符号:  (空格)
		用法: 
			div span{ color: red; }

6. 并集选择器

		符号: ,
		用法: 
			div,p { color: red; }

7. 子代选择器

		符号: > 
		用法: 
			div>span { color: red; }

8. 紧邻选择器

		符号: +
		用法:
			div+p { color: red; }

		选择 div 紧挨着的下一个 p 元素

#### 2. jQuery基本选择器

1. id选择器

		符号: $("#demo")
		用法: $("#demo").css("background","red");
		说明: 选择id为demo的第一个元素

2. 类选择器

		符号: $(".liItem")
		用法: $(".liItem").css("background","red");
		说明: 选择所有类名(样式名)为liItem的元素

3. 标签选择器

		符号: $("div")
		用法: $("div").css("background","red");
		说明: 选择所有 div 标签

4. 通配符选择器

		符号: * 
		用法: $("*").css("background","red");
		说明: 选择所有元素, 少用或者配合其他选择器使用

5. 多元素选择

		符号: $(".liItem,div")
		用法: $(".liItem,div").css("background","red");
		说明: 选择多个指定元素, 选择出类名为.liItem和所有div元素

6. 后代选择器

		符号:  (空格)
		用法: $("div span").css("background","red");
		说明: 后代选择器, 选择所有的后代元素

7. 子代选择器

		符号: > 
		用法: $("div>span").css("background","red");
		说明: 子代选择器, 选择所有的子代元素

8. 紧邻选择器

		符号: + 
		用法: $("div+p").css("background","red");
		说明: 紧邻选择器, 选择紧挨着的下一个元素

9. 兄弟选择器

		符号: ~
		用法: $("div~p").css("background","red");
		说明: 兄弟选择器, 选择后面的所有的兄弟元素

			