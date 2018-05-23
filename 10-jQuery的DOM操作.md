### jQuery的DOM操作

#### jQuery操作样式

1. 设置样式

		$("div").css("background","pink");

2. 添加样式

		$("div").addClass("color-red");

3. 移除样式

#### jQuery操作属性

1. 设置属性

		$("div").attr("title","value");

2. 获取属性

		var attr = $("div").attr("title");
		console.log(attr);

3. 移除属性

		$("div").removeAttr("title");

4. 设置值

		$("div").val("value");

5. 获取值

		var value = $("div").val();
		console.log(value);

6. 设置HTML的内容

		$("div").html("<p>动态的 p 元素</p>");
		会清空原本 div 中的内容

7. 获取HTML的内容

		var content = $("div").html();

8. 设置文本内容

		$("div").text("动态创建的文本");

9. 获取文本内容

		var content = $("div").text();
		console.log(content);

#### jQuery操作节点

**内部插入节点**

1. 在 div 内部的后面追加元素 node

		$("div").append(node);

2. 把 node 追加到 div 内部元素的后面

		node.appendTo("div");

3. 在 div 内部元素的前面追加元素 node

		$("div").prepend(node);

4. 把 node 追加到 div 内部元素的前面

		node.prependTo("div");

**外部插入节点**

1. 在 div 后面添加兄弟节点 node

		$("div").after(node)

2. 在 div 前面添加兄弟节点 node

		$("div").before(node);

3. 把 div 插入到 node 节点的前面

		$("div").insertBefore(node);

4. 把 div 追加到 node 节点的后面

		$("div").insertAfter(node);

**删除节点**

1. 删除元素, 可以删除元素本身

		$("div").remove();

2. 删除子元素

		$("div").empty();
		$("div").html(""); 推荐使用

**复制节点**

1. 复制节点
		
		//参数: 为true, 则事件也会被复制, 否知不复制
		$("div").clone(true);

**包裹节点**

1. 单个包裹

		//用 node 元素包裹 div 元素
		$("div").wrap(node);

2. 所有包裹在一个 node 节点中
		
		//所有的 div 元素分别用 node 元素包裹
		$("div").wrapAll(node);

**替换节点**

1. 替换

		$("div").replaceWith(node);

#### jQuery操作元素

**高度和宽度**

1. 设置高度

		$("div").height("300px");

2. 获取高度

		var height = $("div").height();
        console.log(height);

3. 设置宽度

		$("div").width(300);

4. 获取宽度

		var width = $("div").width();
        console.log(width);

5. 对比CSS

		 console.log("height()方式获取的结果是: " + $("div").height()); // 300 Number类型
         console.log("css('height')方法获取的结果是: " + $("div").css("height")); //300px String类型

**坐标值**

1. 设置坐标值 offset, 设置值后变成相对定位

		$("div").offset({
			"top":"topValue",
			"left":"leftValue"
		});

2. 获取坐标值 offset

		$("div").offset().top;
		$("div").offset().left;

3. 获取坐标值 position, 只能获取不能设置

		$("div").position().top;
		$("div").position().left;

**滚动条**

1. 相对于滚动条的顶部偏移

		$("div").scrollTop();

2. 相对于滚动条的左部偏移

		$("div").scrollLeft();
         