###Spans and Divs

-----

Despite the proliferation of block-level and inline html elements, two reign supreme.

The `<div>` element, a page *division*, and the `<span>` element, a span of text, serve as the arbitrary block and inline element, respectively. 

```
<html>
  <head>
  </head>
  
  <body>
    <div>
        <p>
            This is a paragraph tag within the <span>first</span> div tag.
        </p>
    </div>
    <div>
        <p>
            This is a paragraph tag within the <span>second</span> div tag.
        </p>
    </div>
  </body>
</html  
```

On its own, this code doesn't do much different than using only `<p>` tags and leaving the `<span>`s out.

But, we can add styles to the divs and spans.

```
<html>
  <head>
  </head>
  
  <body>
    <div style="color:red">
        <p>
            This is a paragraph tag within the <span>first</span> div tag.
        </p>
    </div>
    <div style="color:blue">
        <p>
            This is a paragraph tag within the <span>second</span> div tag.
        </p>
    </div>
  </body>
</html  
```