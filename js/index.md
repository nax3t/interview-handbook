# JavaScript

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

# [Back to readme](../readme.md)