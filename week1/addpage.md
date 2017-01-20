After [installing the LAMP stack](lampinstall.md), the AWS server is now serving a webpage to interested browsers at your allocated IP address. The page being served is Apache's default welcome message, which can be easily replaced.

[Use ssh](serveraccess.md) to get into your machine, and then use `cd` to move to Apache's default folder.

`cd /var/www/html/`

Anything in this folder will be served to web browsers. By default `index.html` is provided to web browsers by the server, we often call this a 'homepage'. If you run `ls`, you will find a default `index.html` in this directory which contains the Apache welcome message. Rename it for later reference.

`mv index.html apachewelcome.html`

If you were to visit your IP address now, there would be an error, as the web browser can't find the default `index.html` file. Let's create it and add content.

`touch index.html`

`echo "hello world!" > index.html`

Visiting your IP address now should result in a simple webpage exclaiming "hello world!" 

-----

We can easily replace and append content on your `index.html` with `echo`. Something worth adding other than text might be some links. Links allow individual files to reference one another, and web browsers interpret that as clickable link.



