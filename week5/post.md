###Defining a Custom Post Type

---

With a [repository created](account.md), in the Custom Post Type editor, use the builder to pull-in what kinds of content you expect your page to present. These are called *masks* in Prismic documentation. Let's call our first custom post type `post`. In this screen, we are defining what kinds of content will make up a blog post page. For instance, we might want to have a post `title`,`uid` for search engine purposes, a `hero` image, and `body` text.

When defining `title`, you can allow only `<h1>` elements to automatically apply some formatting when this content is injected into the page.

Ensure that this is a *repeatable* post type so that we can have many instances of it within the Prismic interface. In the future, we will setup *single* post types, which exist exactly once. For instance, your `about` page.

Now, let's [fill in some posts](content.md).

