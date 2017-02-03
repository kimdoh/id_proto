###Box Model

------

Due to historical complications, the `width` of any given element in html may or may not include different properties. For instance, the dimensions of `padding` and `border` properties, which sit outside the actual content of the element, are not included. Consider this example.

```
<html>
<head>
	<link href="reset.css" rel="stylesheet">

	<style>
		
		.series{
			width:30%;
			height:500px;
			border:1px solid darkgray; 
			float:left;
			margin-left:1.25%;
			margin-right:1.25%;
			margin-top:10px;
		}

	</style>
</head>

<body>

	<div class="series"> 
	</div>
	<div class="series"> 
	</div>
	<div class="series"> 
	</div>
	
</body>
</html>
```
