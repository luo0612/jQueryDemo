### jQuery的DOM操作

#### jQuery操作样式

1. 设置样式

		$("div").css("background","pink");

2. 添加样式

		$("div").addClass("color-red");

3. 移除样式

#### jQuery操作属性

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