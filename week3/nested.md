###Nested Positioning

-----

Let's write similar html code to the last example. The only different is that, rather than having two divs in sequence, this example nests one div inside another.

```
<html>
<head>
	
	<style>
		
		#parent{
			width:500px;
			height:500px;
			border:1px solid darkgray;    
		}

		#child{
			width:50px;
			height:50px;
			border:1px solid cyan;    
		}


	</style>
</head>

<body>

	<div id="parent"> 
		<div id="child"> 
		</div>
	</div>
</body>


</html>
