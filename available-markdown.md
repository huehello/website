---
layout: page
title: Available markdown
subtitle: Each post also has a subtitle
gh-repo: g24khanna/Dynamic-Theme-Example
gh-badge: [star, fork, follow]
categories: [android]
tags: [test]
---

You can write regular [markdown](http://markdowntutorial.com/) here and Jekyll will automatically convert it to a nice webpage.  I strongly encourage you to [take 5 minutes to learn how to write in markdown](http://markdowntutorial.com/) - it'll teach you how to transform regular text into bold/italics/headings/tables/etc.

**Here is some bold text**

*How about Italic*

OR ~~Striked text~~

## Here is a secondary heading

Here's a useless table:

| Number | Next number | Previous number |
| :------ |:--- | :--- |
| Five | Six | Four |
| Ten | Eleven | Nine |
| Seven | Eight | Six |
| Two | Three | One |


How about a yummy crepe?

![Crepe](http://s3-media3.fl.yelpcdn.com/bphoto/cQ1Yoa75m2yUFFbY2xwuqw/348s.jpg)


Here's a code chunk:

~~~
var foo = function(x) {
  return(x + 5);
}
foo(3)
~~~

And here is the same code with syntax highlighting:

```javascript
var foo = function(x) {
  return(x + 5);
}
foo(3)
```

And here is the same code yet again but with line numbers:

{% highlight javascript linenos %}
var foo = function(x) {
  return(x + 5);
}
foo(3)
{% endhighlight %}

## Boxes
You can add notification, warning and error boxes like this:

### Notification

{: .box-note}
**Note:** This is a notification box.

### Warning

{: .box-warning}
**Warning:** This is a warning box.

### Error

{: .box-error}
**Error:** This is an error box.

### Plain

{: .box-plain}
When you have to think inside the box!

### Bordered

{: .box-border}
Sometimes things are good with boxed boundary and how about this

### Plain post card
{% include post_card.html title="Checkout Blogs " description="Smart lights have huge potential and we are trying our best to make it easy for you with our blogs. We share ..."
 url="/blogs"
 %}



## Material CARDS


One of my favourite is material card:
{% include material_card.html title="Checkout Blogs " description="Smart lights have huge potential and we are trying our best to make it easy for you with our blogs. We share ..."
 url="/blogs"
imgcss="md-card_image_checkout_blogs"
 %}

 OR two card in grid

 <ul class="grid-two">
 	
{% include material_card.html title="Checkout Blogs " description="Smart lights have huge potential and we are trying our best to make it easy for you with our blogs. We share ..."
 url="/blogs"
imgcss="md-card_image_checkout_blogs"
 %}

{% include material_card.html title="Checkout Blogs " description="Smart lights have huge potential and we are trying our best to make it easy for you with our blogs. We share ..."
 url="/blogs"
imgcss="md-card_image_checkout_blogs"
 %}
</ul>

OR three cards in grid

<ul class="grid-three">
 	
{% include material_card.html title="Checkout Blogs " description="Smart lights have huge potential and we are trying our best to make it easy for you with our blogs. We share ..."
 url="/blogs"
imgcss="md-card_image_checkout_blogs"
 %}

{% include material_card.html title="Checkout Blogs " description="Smart lights have huge potential and we are trying our best to make it easy for you with our blogs. We share ..."
 url="/blogs"
imgcss="md-card_image_checkout_blogs"
 %}

 {% include material_card.html title="Checkout Blogs " description="Smart lights have huge potential and we are trying our best to make it easy for you with our blogs. We share ..."
 url="/blogs"
imgcss="md-card_image_checkout_blogs"
 %}
</ul>


## Youtube Video

{% include youtube.html url="https://www.youtube.com/embed/yv6gl0hIwEU" %}

