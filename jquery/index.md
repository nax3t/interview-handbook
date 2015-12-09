# jQuery

- What is $(document).ready() function? Why should you use it? 
- How do you retrieve attribute of an HTML tag using jQuery e.g. href of links?

Following questions taken from http://www.toptal.com/jquery/interview-questions
- $( "div#first, div.first, ol#items > [name$='first']" )
- The code below is for an application that requires defining a click handler for all buttons on the page, including those buttons that may be added later dynamically. What is wrong with this code, and how can it be fixed to work properly even with buttons that are added later dynamically?
```js
// define the click handler for all buttons
$( "button" ).bind( "click", function() {
    alert( "Button Clicked!" )
});

/* ... some time later ... */

// dynamically add another button to the page
$( "html" ).append( "<button>Click Alert!</button>" );
```

- What’s the deal with the $ in jQuery? What is it and what does it mean?
- How can jQuery be used in conjunction with another JavaScript library that also uses $ for naming?
- Given the following HTML:
```html
<div id="expander"></div>
```
and the following CSS:
```css
div#expander{
  width: 100px;
  height: 100px;
  background-color: blue;
}
```
Write code in jQuery to animate the `#expander` div, expanding it from 100 x 100 pixels to 200 x 200 pixels over the course of three seconds.

- What is method chaining in jQuery? Provide an example. What advantages does it offer?
- Explain what the following code does:
```js
$( "div" ).css( "width", "300px" ).add( "p" ).css( "background-color", "blue" );
```

- What is the difference between jQuery.get() and jQuery.ajax()?
- Which of the two lines of code below is more efficient? Explain your answer.
```js
document.getElementById( "logo" );
```
or
```js
$( "#logo" );
```

- Explain and contrast the usage of `event.preventDefault()` and `event.stopPropagation()`. Provide an example.
- What selector would I use to query for all elements with an ID that ends with a particular string? Also, how would I modify the selector to retrieve only `<div>` elements whose IDs end with that same string? Provide an example.
- What is accomplished by returning `false` from (a) a jQuery event handler, (b) a regular JavaScript onclick event handler for an anchor tag, and (c) a regular JavaScript onclick event handler for a non-anchor tag (e.g., a div, button, etc.)?
- jQuery provides a useful `.clone()` method to create a deep copy of matching elements.
	- Answer the following questions:
		1. What is meant by a “deep copy”?
		2. What is normally not included in the cloned copy? How can some of this behavior be controlled?
		3.What is a potential “gotcha” when using the `.clone()` method? (HINT: What is an element attribute that you would generally not want to clone?)
- Explain the `.promise()` method in jQuery, including how and why it would be used.
- Consider the code snippet below. If there are 5 `<div>` elements on the page, what will be the difference between the start and end times displayed?
```js
function getMinsSecs() {
  var dt = new Date();
  return dt.getMinutes()+":"+dt.getSeconds();
}

$( "input" ).on( "click", function() {
  $( "p" ).append( "Start time: " + getMinsSecs() + "<br />" );
  $( "div" ).each(function( i ) {
    $( this ).fadeOut( 1000 * ( i * 2 ) );
  });
  $( "div" ).promise().done(function() {
    $( "p" ).append( "End time: " + getMinsSecs() + "<br />" );
  });
});
```

# [Back to readme](../readme.md)