ArcMenu
=======

创建弧形菜单

========
#usage
```javscript
<script type="text/javascript" src="arcMenu.js"></script>
<div class="container">
	<a id="toggleMenu" href="#">click me</a>
	<div id="menusBox">
		<a class="menu" href="#">1</a>
		<a class="menu" href="#">2</a>
		<a class="menu" href="#">3</a>
		<a class="menu" href="#">4</a>
		<a class="menu" href="#">5</a>
		<a class="menu" href="#">6</a>
		<a class="menu" href="#">7</a>
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
		// 展开距离
		distance:110
	});
</script>
```
