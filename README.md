Paralmax.js
===========

Paralmax is a JQuery responsive parallax plugin for multiple uses, including full size section background image, page parallax elements and more based on different use cases. With many built-in settings, users can set parallax speed, background image to full size or not, disable it below specific screen size and reset element to the top of it's parent container. The advantage of Paralmax is that it only adds parallax effet to elements, but not changes their style/looking, so users can easily customise/style any elements with pure HTML or CSS (position, size, image, background, content, etc).


### Link to Files

```html
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js" type="text/javascript"></script>
<script src="js/paramax.js" type="text/javascript"></script>
```


### Set up Codes

#### HTML Code

Simply add class .parallax-object to the elements that you want to parallax.

```html
<div class="parallax-object">
    <img src="images/2.jpg" alt="">
</div>
```

#### JQuery Call

```javascript
jQuery(function($){

    // PARALLAX FUNCTIN CALL
    $(".parallax-object").each(function() {
        parallaxObject($(this));
    });

});
```

No built-in CSS is used/necessary, just style your elements to however you like before you parallax them.


### HTML Data Options

#### Speed ( float, from 0.x to x.0 )

0 means the parallax element will be fixed in place, in this case, you don't need Paralmax. 1 means the same speed as page scoll, x.0 Means x times of the page scrolling speed. Default is 0.5.

#### Resize ( boolean, true or false )

Resize ( boolean, true or false )

```html
<div data-resize="true"></div>
```

#### Breakpoint ( boolean, true or false )

Disable paralalx effect while below the specific screen size.

```html
<div data-breakpoint="768"></div>
```