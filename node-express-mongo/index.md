# Node / Express / Mongo

### Node

Questions taken from https://blog.risingstack.com/node-js-interview-questions/

- What is an error-first callback?
- How can you avoid callback hells?
- How can you listen on port 80 with Node?
- What's the event loop?
- What tools can be used to assure consistent style?
- What's the difference between operational and programmer errors?
- Why npm shrinkwrap is useful?
- What's a stub? Name a use case.
- What's a test pyramid? How can you implement it when talking about HTTP APIs?
- What's your favourite HTTP framework and why?

Questions taken from http://www.toptal.com/nodejs/interview-questions

- If we are using Node.js version 0.10 or higher, how else might we write the code below?
```js
console.log("first");
setTimeout(function() {
    console.log("second");
}, 0);
console.log("third");
```
The output will be:
```
first
third
second
```
- What is “callback hell” and how can it be avoided?
- How does Node.js handle child threads?
- What is the preferred method of resolving unhandled exceptions in Node.js?
- How does Node.js support multi-processor platforms, and does it fully utilize all processor resources?
- What is typically the first argument passed to a Node.js callback handler?
- Consider following code snippet. The time required to run this code in Google Chrome is considerably more than the time required to run it in Node.js. Explain why this is so, even though both use the v8 JavaScript Engine.
```js
{
    console.time("loop");
    for (var i = 0; i < 1000000; i += 1){
        // Do nothing
    }
    console.timeEnd("loop");
}
```

# [Back to readme](../readme.md)