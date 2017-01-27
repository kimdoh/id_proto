###Week 1: Block Elements

-----

Inside of Sublime Text, press `command/control + shift + p` to open the command palette. There, type in `Browse Server`, select it, and then select your previously created SFTP configuration file. You should see the contents of your `/var/www/html` directory.

Create a new file called `index.html`. This is the file that browsers load when a website address is visited.

Visit your elastic IP address in a browser, and reload the page after each following step to see the results of you code visualized.

Rather than just typing text into this file as we have done previously, let's begin writing specially formatted HTML code for in-browser rendering.

First, let's declare the document as an html file by wrapping the whole file in the appropriate tag.

```
<html>

</html>
```

Now, let's add a few structural tags that each html document should have.

```
<html>
  <head>
  </head>
  
  <body>
  </body>
</html>
```

The `<head>` tag contains any code or data that *should not be displayed* on the resulting web page. For instance, tags specifying links to necessary scripts, stylesheets, and analytics libraries will be placed inside of the `<head>` tag.

The `<body>` tag contains all of the visible parts of the webpage. Let's add some content!

```
<html>
  <head>
  </head>
  
  <body>
    <h1>Webpage Title</h1>
    <p>
    This is some body text.
    </p>
    <p>
    This is some more body text.
    </p>
  </body>
</html>
```

This should render like this in a browser.

<hr />

<h1>Webpage Title</h1>

This is some body text.

This is some more body text.

<hr />

The `<h1>` element, abbreviated from "first-level-header", adds some default title styling to the text contained within the tags, and `<p>` for simple "paragraph" does not.

There are many levels of headers.

```
<html>
  <head>
  </head>
  
  <body>
    <h1>First Level Webpage Title</h1>
    <h2>Second Level Webpage Title</h2>
    <h3>Third Level Webpage Title</h3>
    <h4>Fourth Level Webpage Title</h4>
    <h5>Fifth Level Webpage Title</h5>
    <h6>Sixth Level Webpage Title</h6>
</body>
</html>
```

<hr />

    <h1>First Level Webpage Title</h1>
    <h2>Second Level Webpage Title</h2>
    <h3>Third Level Webpage Title</h3>
    <h4>Fourth Level Webpage Title</h4>
    <h5>Fifth Level Webpage Title</h5>
    <h6>Sixth Level Webpage Title</h6>

<hr />   
