###Base Code

---

Pulling down data from your Prismic.io API is really easy.

```
<html>
<head>

  <title>Basic Prismic Setup</title>
  
  <meta name="prismic-api" content="https://zap-blog-test.prismic.io/api">

  <script src="js/ejs-1.0.js"></script>
  <script src="js/prismic.io-1.0.10.min.js"></script>
  <script src="js/prismic.io-singlepage-1.0.0.js"></script>
</head>
<body>

</body>
</html>
```

We will need to begin by constructing an html page as normally. We are linking several scripts that allow us to easily implement Prismic calls in the `head` of the page.

The most important line here is the new `<meta>` tag, which is used to embed important information for other web services. Please replace that with a link to your Prismic repository's api.


