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
```

This will render as a cyan square inside a gray square in the upper-left corner of the browser window. We can position the parent div to move it around on the page with `margin-left` and `margin-top`.

```
#parent{
	width:500px;
	height:500px;
	border:1px solid darkgray;    
	
	margin-left:400px;
	margin-top:300px;
}
```

Note that, like with all css properties, rules of inheritance means that the child is moved along with its parent.

The converse is not true.

```
#child{
	width:500px;
	height:500px;
	border:1px solid darkgray;    
	
	margin-left:100px;
	margin-top:300px;
}
```

This positions the child inside of the parent. Inheritance means properties only descend in the tag heirarchy, and never ascend. The child can be moved relative to its parent, just as the parent is moved relative to its parent — the body of the webpage.

Now, let's do some housekeeping and reset our css.
