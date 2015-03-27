ArcMenu
=======

创建弧形菜单

========
#usage

**缓动效果由 菜单项的css transition产生,可随意**

***暂只支持高级浏览器***

```javascript
<script type="text/javascript" src="arcMenu.js"></script>
<div class="container" id="con1">
	<a class="toggle" id="toggleMenu" href="javascript:;">click me</a>
	<div class="box" id="menusBox">
		<a class="menu" href="javascript:;">1</a>
		<a class="menu" href="javascript:;">2</a>
		<a class="menu" href="javascript:;">3</a>
		<a class="menu" href="javascript:;">4</a>
		<a class="menu" href="javascript:;">5</a>
	</div>
</div>
<div class="container" id="con2">
	<a class="toggle" id="t1" href="javascript:;">click me</a>
	<div class="box" id="m1">
		<a class="menu" href="javascript:;">1</a>
		<a class="menu" href="javascript:;">2</a>
		<a class="menu" href="javascript:;">3</a>
		<a class="menu" href="javascript:;">4</a>
	</div>
</div>
```

	var menu=new arcMenu({
		// 开关按钮
		menu_btn:"toggleMenu",
		// 按钮组父元素
		menu_box:"menusBox",
		// 起始角度 0-360
		start_angel:-10,
		// 总角度0-360
		total_angel:110,
		// 是否旋转菜单
		isRotate:true,
		// 默认是否打开
		isActive:true,
		// 展开菜单时候
		openEvt:function(){},
		// 菜单关闭的时候
		openEvt:function(){},
		// 展开距离
		distance:110
	});

	var container1=document.getElementById("con1");
	var container2=document.getElementById("con2");
	// 外部控制开关
	container1.addEventListener("click",function(){
		menu.close();
	},false);
	container2.addEventListener("click",function(){
		menu2.close();
	})

	var menu2=new arcMenu({
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


