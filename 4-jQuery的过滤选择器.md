### jQuery过滤选择器

1. 选择序号第一个匹配制定索引index的元素

		符号: :eq(index)
		用法: $("li:eq(1)").css("background","red");
		说明: 索引index从 0 开始, 选择序号为index的元素. 选择第一个匹配的元素

2. 选择序号大于指定索引index的元素

		符号: :gt(index)
		用法: $("li:gt(2)").css("background","red");
		说明: 索引index从 0 开始, 选择序号大于index的元素

3. 选择序号小于制定索引index的元素

		符号: :lt(index)
		用法: $("li:lt(2)").css("background","red");
		说明: 索引index从 0 开始, 选择序号小于index的元素

4. 选择序号为奇数的元素

		符号: :odd
		用法: $("li:odd").css("background","red");
		说明: 选择序号为奇数的元素

5. 选择序号为偶数的元素

		符号: :even
		用法: $("li:event").css("background","red");
		说明: 选择序号为偶数的元素

6. 选择匹配的第一个元素

		符号: :first
		用法: $("li:first").css("background","red");
		说明: 选择匹配的第一个元素

7. 选择匹配的最后一个元素

		符号: :last
		用法: $("li:last").css("background","red");
		说明: 选择匹配的最后一个元素