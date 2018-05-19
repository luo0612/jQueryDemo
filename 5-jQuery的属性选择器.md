### jQuery的属性选择器
	
1. 选择包含所有 attribute 属性的元素

		符号: $("element[attribute]")
		用法: $("a[href]").css("background","red");
		说明: 选择所有包含 href 属性的元素

2. 选择 attribute 属性值为指定值的所有元素

		符号: $("element[attribute='value']")
		用法: $("a[href='itcast']").css("bacground","red");
		说明: 选择 href 属性值为 itcast 的所有 a 标签

3. 选择 attribute 属性值不为指定值的所有元素

		符号: $("element[attribute!='value']")
		用法: $("a[href!='baidu']").css("bacground","red");
		说明: 选择所有 href 属性值不等于 baidu 的所有 a 标签, 包含没有 href 的元素

4. 选择 attribute 属性值为指定值开头的所有元素

		符号: $("element[attribute^='value']")
		用法: $("a[href^='web']").css("background","red");
		说明: 选择所有 href 属性值以 web 开头的所有 a 标签

5. 选择 attribute 属性值以指定值结尾的所有元素

		符号: $("element[attribute$='value']")
		用法: $("a[href$='cn']").css("background","red");
		说明: 选择所有 href 属性值以 cn 结尾的所有 a 标签

6. 选择 attribute 属性值包含指定值的所有元素

		符号: $("element[attribute*='value']")
		用法: $("a[href*='i']").cas("background","red");
		说明: 选择所有 href 属性值包含 i 的所有 a 标签, 可以是中英文

7. 选择所有 attribute 属性和属性值都符合的所有元素

		符号: $("element[attribute][attribute='value']")
		用法: $("a[href][title="我"]").css("background","red");
		说明: 选择含有 href 属性和 titile 的属性值为 "我" 的所有 a 标签, 都符合才会被选中