###Base Code

---

Pulling down [your content](content.md) from your Prismic.io API is really easy. But first we need a shell to hold it.

```
<html>
<head>

  <title>Basic Prismic Setup</title>
  
  <meta name="prismic-api" content="https://##########.prismic.io/api">

  <script src="js/ejs.js"></script>
  <script src="js/prismic.min.js"></script>
  <script src="js/prismic.singlepage.js"></script>
</head>
<body>

</body>
</html>
```

We will need to begin by constructing an html page as normally. We are linking several scripts that allow us to easily implement Prismic calls in the `head` of the page.

These files can be found below. Make sure you place them in a `js` directory.

- [ejs.js](ejs.js)
- [prismic.min.js](prismic.min.js)
- [prismic.singlepage.js](prismic.singlepage.js)

The most important line here is the new `<meta>` tag, which is used to embed important information for other web services. Please replace that with a link to your Prismic repository's api.

We can now [reach out](call.md) to the Primic api.
