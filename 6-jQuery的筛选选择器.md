### jQuery的筛选选择器

1. 选择序号等于指定 index 值的第一个元素

		符号: .eq(index)
		用法: $("span").eq(1).css("background","red");
		说明: 类比 ":eq(1)" 选择器, 元素的序号从 0 开始计算, 选择序号等于指定 index 值的元素

2. 选择指定元素的第一个元素

		符号: .first()
		用法: $("span").first().css("background","red");
		说明: 类比 ":first"选择器, 选择指定元素的第一个元素

3. 选择指定元素的父元素

		符号: .parent("value")
		用法: 
			$("#sp").parent().css("background","red");
		说明: 选择 id 为 sp 的元素的父元素

		用法:
			$("p").parent().css("background","red");
		说明: 选择所有 p 标签的父元素

		用法:
			$("p").parent("#div").css("background","red");
		说明: 选择所有 p 标签的父元素中 id 为 div 的父元素

4. 选择指定元素的所有兄弟元素

		符号: .siblings(["value"])
		用法: $("#li").slibings(".liItem").css("background","red")	
		说明: 选择 id 为 li 的所有兄弟元素中 id 为 liItem的元素

5. 查找所有的后代元素

		符号: .find("value")
		用法: $("div").find("#li").css("background","red");
		说明: 选择所有 div 标签的后代元素中 id 为 li 的元素
		