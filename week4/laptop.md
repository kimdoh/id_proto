###Laptops

---

The laptop style rules bring in all elements, and allows for more display flexibility. 

```
/* Laptops: Full, Half, Third, Quarter Widths */
 @media only screen 
 and (min-width : 1024px) 
 and (max-width : 1223px) {
       #container {background-color:#dee;}
      .one { width:15.666%; }
      .two { width:15.666%; }
      .three { width:24% }
      .four { width:32.333%}
      .five { width:40.666% }
      .six { width:49%; }
      .seven { width:57.333%; }
      .eight { width:65.666%; }
      .nine { width:74%; }
      .ten { width:82.333%; }
      .eleven { width:82.333%; }
      .twelve { width:99%; }
  }
  
  The laptop max breakpoint is `1px` less than the desktop `min-width` assigned earlier, and so our grid flows nicely on browser resizing on large displays.
  
  We're done!
