/***css3简单动画效果(对象沿着边框移动)*还没写兼容*如果要兼容要自己写*/
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<style>
	.box1{width:300px;height:300px;border:solid 1px red;position:relative;}
	.subbox{width:20px;height:20px;background:blue;position:absolute;transition:all;transition:all 1s linear;animation:run infinite 3s;}
	
	@keyframes run{
		12.5%{
			top:0px;
			left:140px;
		}
		25%{
			top:0px;
			left:280px;
		}
		50%{
			top:280px;
			left:280px;
		}
		75%{
			top:280px;
			left:0px;
		}
		100%{
			top:0px;
			left:0px;
		}
	}
</style>
<title>rung</title>
</head>

<body>

<div class="box1">
	<div class="subbox"></div>
</div>

</body>
</html>
