### jQuery的动画

#### 基本效果(显示和隐藏)

1. 让 div 显示

		$("div").show();

2. 让 div 隐藏

		$("div").hide();

#### 滑动效果

1. 下拉显示

		$("div").slideDown();

2. 上拉显示

		$("div").slideUp();

3. 下拉上拉切换

		$("div").slideToggle();

#### 浅入浅出

1. 淡入

		$("div").fadeIn();

2. 淡出

		$("div").fadeOut();

3. 淡入淡出切换

		$("div").fadeToggle();

4. 淡入到指定透明度

		// 参数2: 设置不透明度, 0.0~1.0
		$("div").fadeTo(2000, 0.1);	

#### 自定义动画

1. 自定义动画

		$("div").animate({
			"width":"500px",
			"height":"600px"
			/* 
			  自定义动画不支持背景颜色的动画,
			  如果需要支持背景颜色的动画,
			  需要使用jQuery.Color()插件 
			 */
		},2000);	

2. 停止动画

		//参数1: 设置为true, 则清空动画队列. 立即结束动画, 后面所有的动画都不再执行. 默认值为false
		//参数2: 设置为true, 让当前正在执行的动画立即执行完成, 后面的动画继续执行, 最后重置show和hide的原始样式,调用回调函数等. 默认为false
		$("div").stop(false, true);
