###Positioning

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

You should now see a thin gray rectangle in the upper left corner of the page.

