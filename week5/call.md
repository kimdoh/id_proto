###Accessing Prismic Content

---

Once Prismic is [properly linked](base.md), we can easily query the Prismic API.

Using a go-between helping language called [ejs.js](http://www.embeddedjs.com), we can store javascript information in html variables. This code belongs in the body of your page.

```
<script type="text/prismic-query" data-binding="posts">

    [
    [:d = at(document.type, "post")]
    ]

</script>
```

The `data-binding` attribute of our script allows us to reuse the literal `posts` to reference the results of the script itself. Here, we are asking Prismic to return to us any content that has the `type` of `post`. 

`posts` now holds the results from the prismic api call. Let's use it below.

```
<h1>[%= posts.length %] Posts are Available!</h1>

  [% posts.forEach(function(post) { %]

    <div>
      <h2>[%= post.getText('post.title') %]</h2>
      <img data-src="[%= post.getImageView('post.hero', 'main').url %]">
      <p>
           [%= post.getText("post.body") %]
      </p>
      <hr />
    </div>
  [% }) %]
```

The `forEach` will execute once per returned javascript object. In this case, it will execute once for each `post` in the Prismic interface. We use ejs.js brackets to intermix calls for specific prismic information with literals and html structure.
