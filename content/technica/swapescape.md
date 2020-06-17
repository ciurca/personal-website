---
title: "How to swap the Escape key with Capslock in Ubuntu"
date: 2020-06-17
description: "Make a powerful key more accessible."
tags: ['vim', 'ubuntu']
images: ['/img/tehnica/escape.jpg']
draft: false
---

[Jump to the way of doing this](#the-way)

## But why?

If you've started or have been using VIM for some while now, you know that the Escape key has significant value.

Staying in the home row, also has significant value, so swapping the Escape key with Capslock is the natural thing to do.

The Capslock key is more accessible, so you don't have to move your whole hand just to press Escape. You can simply use your pinky finger.

## Swapping vs remapping

We're swapping the Escape and Capslock key, meaning that if you want to press Escape, you'll now have to press Caps and vice-versa. I've seen tutorials that remap the Escape key, leaving you with no Caps key, so this method just seemed easier.

## The way

We're going to use the **dconf** command to swap the two keys.

Simply run this command in your terminal:

```
dconf write /org/gnome/desktop/input-sources/xkb-options "['caps:swapescape']"
```

**Special note**: I found the way of doing this in [this](http://disq.us/p/1msufl0) comment on [this](https://era86.github.io/2017/01/14/remapping-capslock-to-escape-in-ubuntu-1604.html) tutorial on how to remap Capslock to Escape.

{{< rawhtml >}}
Meta Photo by <a href="https://unsplash.com/@charlesdeluvio?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">Charles Deluvio</a> on <a href="/s/photos/escape?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">Unsplash</a>
{{< /rawhtml >}}
