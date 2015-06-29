---
title: Semantic Tags
date: 2015-06-25 22:56:00 -0400
layout: post
---

One of my struggles with Project 1 (Build a Portfolio Site) was understanding
HTML5 semantic tags. I had an idea on their meaning and purpose, but putting
them into practice, I was a bit lost.


### Syntax vs. Semantics ###

Understanding what "semantic" means is important. Actually, "semantic" is all
about what the meaning of something is.

Taking an example from the [Intro to the Semantic Web](https://www.youtube.com/watch?v=OGg8A2zfWKg)
video on YouTube, compare the following:

> I love technology.

> I ♥ technology.

They are written different ways (different syntax), but they hold the same
meaning (same semantics). Does that make sense?


### Pre-HTML5 Semantic Tags ###

Semantic tags are not a new thing. In fact, some have existed since the early
days of the internet. You're more than likely using some already.

What makes a tag semantic? It's a tag that provides information on what is
contained within the element. It tells you what that is supposed to represent or
be. Again, semantics are about meaning.

We have paragraph tags (`p`), for instance. When you see that tag what do you
expect to be in it? A paragraph, right?

Header tags (`h1`, `h2`, etc.) are for headers in different sections, each
at a different level. You see words within such tags, and you know that it is a
title to an area and just how major of an area it is.

What about `div` or `span`? These tags don't tell you anything about the
content. They're just groupings. They serve a purpose and are useful, but they
are not semantic.


### HTML5 Semantic Tags ###

Well, `div` is all over the place and is rather useful. What if we could just
make tags like it that were semantic? HTML5 kind of did that.

Take this example:

```html
<body>
  <div class="grid">

    <div class="row">
      <div class="col-6">
        <img class="image" src="/img/logo.png" alt="logo">
        <h1>Site Title</h1>
      </div>
      <div class="col-6">
        <p>Tagline</p>
      </div>
    </div>

    <div class="row">
      <div class="col-12">
        <h2>Article Title</h2>
      </div>
    </div>

    <div class="row">
      <div class="col-12">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit.
          Illo dolorum nemo cumque cum consequatur sed est reiciendis
          voluptas soluta suscipit corrupti aperiam, unde, ullam
          veritatis vel ducimus dignissimos sunt omnis.
        </p>
      </div>
    </div>

    <div class="row">
      <div class="col-12">
        <h2>Another Article Title</h2>
      </div>
    </div>

    <div class="row">
      <div class="col-12">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit.
          Illo dolorum nemo cumque cum consequatur sed est reiciendis
          voluptas soluta suscipit corrupti aperiam, unde, ullam
          veritatis vel ducimus dignissimos sunt omnis.
        </p>
      </div>
    </div>

  </div>
</body>
```

With some looking over, you can get an idea of what's going on here, right? It's
a page with a heading at the top. After that comes an article heading, and then
the article. Then we get another one after that.

Let's try some HTML5 tags.

```html
<body>
  <div class="grid">

    <header class="row">
      <div class="col-6">
        <img class="image" src="/img/logo.png" alt="logo">
        <h1>Site Title</h1>
      </div>
      <div class="col-6">
        <p>Tagline</p>
      </div>
    </header>

    <main>

      <article>
        <div class="row">
          <div class="col-12">
            <h2>Article Title</h2>
          </div>
        </div>

        <div class="row">
          <div class="col-12">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing
              elit. Illo dolorum nemo cumque cum consequatur sed
              est reiciendis voluptas soluta suscipit corrupti
              aperiam, unde, ullam veritatis vel ducimus
              dignissimos sunt omnis.
            </p>
          </div>
        </div>
      </article>

      <article>
        <div class="row">
          <div class="col-12">
            <h2>Another Article Title</h2>
          </div>
        </div>

        <div class="row">
          <div class="col-12">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing
              elit. Illo dolorum nemo cumque cum consequatur sed
              est reiciendis voluptas soluta suscipit corrupti
              aperiam, unde, ullam veritatis vel ducimus
              dignissimos sunt omnis.
            </p>
          </div>
        </div>
      </article>

    </main>

  </div>
</body>
```

Don't you think it's easier to see what's going on with those tags saying what
each area is supposed to be?

Now, I did this particular example for a reason. If you compare the two, you'll
see that I've not just replaced `div` tags, I've wrapped some in the new tags.
It gets confusing if you think you have to _always_ replace `div` tags.

Replace some, wrap some, do whatever makes sense to you. Remember, making sense
of what you're coding is what these semantic tags are all about. :smile:


### Links ###

For more details on specific tags, and more examples, check these links out:

 * ["HTML5 Semantic Elements" by W3Schools](http://www.w3schools.com/html/html5_semantic_elements.asp)
 * ["How to Use The HTML5 Sectioning Elements" by Treehouse](http://blog.teamtreehouse.com/use-html5-sectioning-elements)
 * ["Let's Talk About Semantics" by HTML5 Doctor](http://html5doctor.com/lets-talk-about-semantics/)
 * [Content Sectioning of "HTML Element Reference" by Mozilla](https://developer.mozilla.org/en-US/docs/Web/HTML/Element#Content_sectioning)
