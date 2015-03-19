ArcMenu
=======

创建弧形菜单

========
#usage

**缓动效果由 菜单项的css transition产生,可随意**

***暂只支持高级浏览器***

```javscript
<script type="text/javascript" src="arcMenu.js"></script>
<div class="container">
	<a class="toggle" id="toggleMenu" href="#">click me</a>
	<div class="box" id="menusBox">
		<a class="menu" href="#">1</a>
		<a class="menu" href="#">2</a>
		<a class="menu" href="#">3</a>
		<a class="menu" href="#">4</a>
		<a class="menu" href="#">5</a>
		<a class="menu" href="#">6</a>
		<a class="menu" href="#">7</a>
	</div>
</div>
<div class="container">
	<a class="toggle" id="t1" href="#">click me</a>
	<div class="box" id="m1">
		<a class="menu" href="#">1</a>
		<a class="menu" href="#">2</a>
		<a class="menu" href="#">3</a>
		<a class="menu" href="#">4</a>
	</div>
</div>
<script type="text/javascript">
	var menu=new arcMenu({
		// 开关按钮
		menu_btn:"toggleMenu",
		// 按钮组父元素
		menu_box:"menusBox",
		// 起始角度 0-360
		start_angel:45,
		// 总角度0-360
		total_angel:140,
		// 是否旋转菜单
		isRotate:true,
		// 默认是否打开
		isActive:false,
		// 展开菜单时候
		openEvt:function(){},
		// 菜单关闭的时候
		openEvt:function(){},
		// 展开距离
		distance:110
	});

	// 创建直线菜单
	new arcMenu({
		// 开关按钮
		menu_btn:"t1",
		// 按钮组父元素
		menu_box:"m1",
		// 起始角度 0-360
		start_angel:0,
		// 总角度0-360
		total_angel:90,
		// 是否旋转菜单
		isStraight:true,
		// 默认是否打开
		isActive:false,
		// 展开菜单时候
		openEvt:function(){},
		// 菜单关闭的时候
		openEvt:function(){},
		// 展开距离
		distance:250
	});
</script>
```
