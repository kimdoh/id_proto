###Concepts

---

We have focused so far on layout, via a responsive HTML grid system, and styling, through CSS properties and media queries.

As a result, we have left *content* mostly untouched. Content is obviously the heart of any website, and no amount of beautiful page structure and styling can substitute for robust content stores.

In the early days of the internet, HTML layout, CSS styling rules, and content all lived together in single a document via inline definitions and table-based layouts. These were the dark days, when editing a website meant wading through line after delicate line of intermixed layout code, styling rules, dynamic code, and content.

Early on in the development of the modern internet, `<link>` and `<script>` tags allowed the separation of CSS from the main html documents. This was a huge moment that helped trigger the first wave of the internt's popularity in the early aughts.

Content, however, had stubbornly remained inextricably nested within html layouts. This changed with the advent of PHP, a language that allowed content to be injected into html layout templates. This is now known as the *web 2.0* phase of the internet.

PHP is a difficult language to learn, however, which has left the situation less than ideal. Giant PHP Content Management Systems [CMS] attempted to disguise all of the complexity inherent to injected content and provide better content creation experiences, but those must often relied on fragile database solutions to store metadata. If something goes wrong, data is permanently lost. [Wordpress](http://www.wordpress.org), powering 26% of the internet as of November, 2016, is the most widespread example of this, though within the design world we are perhaps more familiar with [Squarespace](http://www.squarespace.com).

But, moving forward, these large, immovable systems are not forward-looking. Services like [Apostrophe.js](http://apostrophecms.org), [Contentful.js](https://www.contentful.com), and [Prismic.io](http://www.prismic.io) have finally separated content from layout, providing significantly more flexible website-building and -maintaining experiences.  

These services are called *headless* CMS systems. We use these systems' websites to construct our content, and they masquerade as APIs with a structured query language. We request our content from their servers, and inject it into our layouts.

Let's set an account up on [Prismic.io](http://www.prismic.io) to see how this new system works.
