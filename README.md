# JS Libraries
## Intro

A JavaScript library is prewritten JavaScript code that allows for easy integration to streamline your own code base

There are many JavaScript libraries designed for different purposes. Jasmine is the library we use for writing tests. D3.js is a library for data visualization, Bootstrap has a JavaScript library for adding animations and effects to our sites, Node.js is a library for writing server side JavaScript.

One of the most widely used JavaScript libraries is **jQuery**.

##Objectives
After this lesson you will understand
*Why we use jQuery
*How to link to external libraries like jQuery

##jQuery

jQuery provides us with convenient methods to make our jobs as developers much easier - we can write significantly fewer lines of code and still achieve the same effect.

For example, when we were looking at Twitter and replacing names, we used jQuery:
```
names = $('.fullname');
names.text('Your Name');
```
Without the jQuery library, we would have needed to write:
```
names = document.getElementsByClassName("fullname");
for ( i = 0 ; i < names.length() ; i++ ) {
     names[ i ].innerHTML = " [your name] "
}
```
Underneath the hood, jQuery is just JavaScript, but with build-in methods that simplify our code and enhance readability.

In past projects, most students have primarily used jQuery for event handling and animation, but it's important to have some familiarity with the gamut of jQuery methods. jQuery can be used for four main applications, the first three of which are covered in this prework.

* DOM Manipulation - accessing and changing the structure of a page's HTML or CSS.
* Event Handling - responding to user events like loading a page or clicking a button
* Animation - adding custom effects
* AJAX interaction - processing small bits of data without reloading the page

Importantly, jQuery is also an open source library and has a tremendous community around it. At the time of this writing, over [78% of the top million sites on the web use jQuery](http://trends.builtwith.com/javascript/jQuery) - crazy!

## Using External Libraries
To include JavaScript into your HTML page, use the `<script>` tag. When you want to use an external library like jQuery, point the src attribute to the url of the library you want to use. Like this:

```html
<script src=“https://cdnjs.cloudflare.com/ajax/libs/jquery/2.1.4/jquery.js”></script>
```
Notice that the url points us to a Javascript file, `jquery.js`. If you [look at that file](https://cdnjs.cloudflare.com/ajax/libs/jquery/2.1.4/jquery.js), you can see the JavaScript framework the makes up jQuery.

When you add a script tag that links your page to the jQuery libray, you can now use jQuery methods locally, including the select `$()` and `.text()` methods that we saw in the Twitter example.

## Summary

jQuery takes common tasks that require many lines of JavaScript code to accomplish, and wraps them into methods that you can call with a single line of code. We'll dive deeper into using jQuery in the next few lessons.
