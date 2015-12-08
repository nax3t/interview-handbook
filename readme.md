
### Galvanize Interview Handbook

The purpose of this repo is for you to practice answering interview questions and to refresh your knowledge of some key concepts in HTML, CSS, JavaScript, Ruby, Angular and programming as a whole. 

Pull requests with all of these answers should be submitted by the time the cohort ends. 

### [HTML](../../html)

### CSS
Questions from https://github.com/developerquestions/css-questions
- What are the pros and cons of using absolute positioning?
- What is the difference between display: inline; and display: inline-block;?

Questions from https://github.com/bargitta/cssInterview
- What is box model?
- Where to define styles?
- List CSS selectors and their priorities
- The difference between block element, inline-block element and inline element
- Talk about position property, and its values
- How to hide an element?
- What is float element?
- What is pseudo element? what is pseudo class?
- How to center align a paragraph?
- How to center align a div inside another div?
- How to make a two column Web page? a three column Web page?
- How to draw a triangle? a circle? a colored square?
- How to make a tab view?

Questions from https://css-tricks.com/interview-questions-css/
- Using CSS properties alone, recreate this button:

![CSS Button](./css-button.png)
- Describe what a “reset” CSS file does and how it’s useful. Are you familiar with normalize.css? Do you understand how they differ?
- What are the various techniques for clearing floats?
- What are sprites and why would use them? How do you go about creating them? What are possible alternatives to sprites?
- What are some accessibility concerns that come up in CSS?
- What tools do you use for cross-browser testing?
- Say you found a rendering problem on one of your sites in Internet Explorer 8, which you have decided you are supporting. How would you approach fixing it?
- What is responsive design all about?
- Have you ever worked with a grid layout? What are your thoughts on that?
- What are the benefits of SVG?
- Say you were tasked with coding a design that used non-standard web fonts, how would you go about it?
- Explain to me what's going on in this CSS selector:
```css
[role=navigation] > ul a:not([href^=mailto]) {

}
```

Questions from http://www.skilledup.com/articles/25-css-interview-questions-answers
- Explain what a class selector is and how it’s used
- What are pseudo classes and what are they used for?
- Explain the three main ways to apply CSS styles to a Web page
- What is grouping and what is it used for?
- What is an ID selector and how is it used?
- What is a Class selector and how does it differ from an ID selector?
- What are child selectors?
- What are the different CSS properties used to change dimensions and what values can they accept?
- How is the float property implemented in CSS?
- How to restore the default property value using CSS?
- What is the purpose of pseudo-elements and how are  they made?
- What is the purpose of the z-index and how is it used?
- What are the advantages and disadvantages of External Style Sheets?
- Explain the difference between visibility:hidden and display:none
- What are some of the new features and properties in CSS3?
- Why shouldn’t I use fixed sized fonts?
- Which font names are available on all platforms?
- What are the advantages/disadvantages of using CSS preprocessors? (SASS, Compass, Stylus, LESS)
- Why and how are shorthand properties used? Give examples.

### JavaScript

- See [here](https://github.com/malachaifrazier/JavaScript-Interview-Questions) for some JS interview exercises
- Questions below from https://github.com/nishant8BITS/101-JavaScript-Interview-Question
- Difference between undefined and not defined in JavaScript
- What will be the output of below code?

```js
var y = 1;
if (function f(){}) {
  y += typeof f;
}
console.log(y);
```

- What is drawback of creating true private in JavaScript?
- What is “closure” in javascript? Provide an example?
- Write a mul function which will properly when invoked as below syntax:

```js
console.log(mul(2)(3)(4)); // output : 24 
console.log(mul(4)(3)(4)); // output : 48
```

- How to empty an array in JavaScript?
- How to check if an object is an array or not?
- What will be the output of below code?
```js
var output = (function(x){
  delete x;
  return x;
})(0);

console.log(output);
```

- What will be the output of below code?
```js
var x = 1;
var output = (function(){
  delete x;
  return x;
})();

console.log(output);
```

- What will be the output of below code?
```js
var x = { foo : 1};
var output = (function(){
  delete x.foo;
  return x.foo;
})();

console.log(output);
```

- What will be the output of the below code?
```js
var Employee = {
  company: 'xyz'
}
var emp1 = Object.create(Employee);
delete emp1.company
console.log(emp1.company);
```

- What is undefined x 1 in JavaScript?
- What will be the output of below code?
```js
var trees = ["xyz", "xxxx", "test", "ryan", "apple"];
delete trees[3];
console.log(trees.length);
```

- What will be the output of below code?
```js
var bar = true;
console.log(bar + 0);   
console.log(bar + "xyz");  
console.log(bar + true);  
console.log(bar + false);
```

- What will be the output of below code?
```js
var z = 1, y = z = typeof y;
console.log(y);
```

- What will be the output of below code?
```js
// NFE (Named Function Expression
var foo = function bar() { return 12; };
typeof bar();
```

- What is the difference between declaring a function in below format?
```js
var foo = function() {
  // Some code
};

function bar() {
  // Some code
};
```

- What is function hoisting in JavaScript?
- What will be the output of below code?
```js
var salary = "1000$";

(function () {
  console.log("Original salary was " + salary);

  var salary = "5000$";

  console.log("My New Salary " + salary);
})();
```

- What is the instanceof operator in JavaScript?
- What would be the output of below code?
```js
function foo() {
  return foo;
}
new foo() instanceof foo;
```

- How do we calculate the length of the associative array below?
```js
var counterArray = {
  A : 3,
  B : 4
};
counterArray["C"] = 1;
```

- What is the difference between Function, Method and Constructor calls in JavaScript?

### jQuery

- What is $(document).ready() function? Why should you use it? 

- How do you retrieve attribute of an HTML tag using jQuery e.g. href of links? 


### Node / Express / Mongo

### Ruby

### Angular

### Programming Concepts / Terms

- What is minification?
- What is continuous integration?
- What is isomorphic JavaScript?
- What are your favorite features about ES2015?


### Computer Science / Data Structures + Algorithms

### Challenges 


