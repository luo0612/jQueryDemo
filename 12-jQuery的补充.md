## jQuery的补充

### 链式编程: end()补充

### 隐式迭代

### map()函数

### each()函数

### noConflict()全局对象污染冲突

	$ jQuery
	
	var $ = {name:"luo"}
	<script src="jquery-3.3.1.js"></script>
	后面的jQuery中的$对象会覆盖掉上面自定义var定义的$对象

	$.noConflict():让jQuery释放$, 让$回归到jQuery之前的对象定义上去, 
	即再次调用使用的是自定义var的$对象

### jQuery.data() jQuery对象的数据缓存

	该方法可以将数据缓存到jQuery的内存中, 并可以获取使用
	
	//缓存数据	
	$(".li").data("name":"123");
	//获取数据
	var t = $(".li").data("name");
	t.name="18";//对象的更改会直接同步到元素的jQuery对象中

### jQuery的插件

#### jQuery的方式

**全局jQuery函数扩展方式**

	$.log=function(){

	};

#### 引入jQuery第三方插件

步骤:

*	引入jQuery
*	引入第三方插件
*	用第三方插件实现效果

**背景色动画插件**

**lazyload插件**

**jQuery UI插件**
	
