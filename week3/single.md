###Simple Positioning

-----

Setup a basic html file.

```
<html>
  <head>
  </head>

  <body>
  </body>
</html
```

Recall that an html file needs a `<head>` and `<body>` tag to be valid.

Let's create an arbitrary page division, a `<div>`, inside of the body of the page and give it a name. Let's also assign an ID for easier styling.

```
<body>
  <div id="positioning">
  </div>
</body>
```

In the head of the page, assign some styles so we can see the div.

```
<head>
  <style>
    #positioning{
		width:50px;
		height:100px;
		border:1px solid darkgray;    
    }
  </style>
</head>
```

The syntax for the css `border` property shorthand used here is `border: strokeweight strokestyle color`. 

You should now see a thin gray rectangle in the upper left corner of the page.

We can move this rectangle around with some useful css positioning properties. There are many options available, we'll focus on the standards.

```
<head>
  <style>
    #positioning{
		width:50px;
		height:100px;
		border:1px solid darkgray;    
		
		margin-left:100px;
		margin-top:20px;
}
  </style>
</head>
```

Using different kinds of units in those `margin` properties allows for more flexiblity. For instance, we can use `%` units to specify the dimensions and positions of items relative to the *width* of the screen.


```
<html>
<head>
	
	<style>
		#positioning{
			width:50px;
			height:100px;        
			border:1px solid darkgray;    
			
			margin-left:10%;
			margin-top:20%;
		}
	</style>
</head>

<body>

<div id="positioning"> 
</div>

</body>


</html>
```
