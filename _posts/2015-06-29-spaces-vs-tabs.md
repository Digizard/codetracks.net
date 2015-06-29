---
title: Spaces vs. Tabs
date: 2015-06-29 13:41:00 -0400
layout: post
---

One of the decisions you have to make when starting your own project (if you
want to write good code) is whether to use spaces or tabs for indenting.

It really is a matter of preference, and you might also find that your taste
varies with the particular project or language you're working with.

Text editors and IDEs today try to be useful for all of their users, and in
that, features such as using the tab key to put in a set amount of spaces
instead or even converting a page's indents from spaces to tabs (and vice versa)
exist.

Whether you choose to do tabs, 2 spaces, 4 spaces, or whatever, you just have to
be consistent. That means you only do a tab, 2 spaces, 4 spaces, etc., each time
you indent.

Exceptions can exist if you are trying to align particular lines of code a
certain way. For instance:

```JavaScript
return isThis ||
       isThat ||
       isCat;
```

To make the this line up with spaces, it takes 7 spaces. That's not divisible
naturally by any set of space choices other than 7 (which would be a weird
number to pick, but hey, if you're consistent).

Using tabs, it takes one tab plus 3 spaces.

If your purpose for not sticking to your choice is because you are trying to
line things up for what you think is better readability, that's fine. :smile:
Just be consistent with that choice, too, and do that every time.

When you work on someone else's project, you'll have to go by their choice. They
might be pickier about sticking to their choice and not let you adjust for nice
line-ups like the above. That's OK. When it's someone else's project, you do
what they decided, just like someone joining your project later would have to do
what you decided.

At the end of the day, it's all just personal preference and not something to
get hung up about. It's not too different from having a favorite color. Trying
to make someone change their favorite color or the color of their house seems
silly, doesn't it? :laughing: