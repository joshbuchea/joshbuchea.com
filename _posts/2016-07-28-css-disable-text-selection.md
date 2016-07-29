---
layout: post
title: Disable Text Selection with CSS
---

{% highlight css %}
.disable-selection {
  -webkit-touch-callout: none; /* Disable Android and iOS callouts*/
    -webkit-user-select: none; /* Chrome, Safari, and Opera */
       -moz-user-select: none; /* Firefox */
        -ms-user-select: none; /* Internet Explorer */
}
{% endhighlight %}
