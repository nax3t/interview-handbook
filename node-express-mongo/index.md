# Node / Express / Mongo

### Node

Questions taken from https://blog.risingstack.com/node-js-interview-questions/

- What is an error-first callback?
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

### Express

Questions from week 6 assessment:
- What is the difference between a host object and a native object?
- Name two objects that are NOT available to us in Node.js (that are available in the browser).
- What is Express JS?
- What is npm?
- What `package.json`?
- Why do we add the text `"node_modules"` to our `.gitignore`?
- What does the --save flag do when we install modules with npm?
- What is nodemon? Why is it so helpful?
- What is localhost?
- What is HTTP?
- Explain GET request vs POST request
- Explain render vs redirect
- What is a route?
- What is EJS?
- Where do static assets (images, javascripts, stylesheets) go?
- What is the difference between `require("express")` and `require("./express")`?
- What is middleware?
- What does `body-parser` enable us to do?
- What is the difference between `req.params`, `req.query` and `req.body`?
- Given the following code:
```js
app.get("/",function(req,res){
    var instructors = ["Matt", "Ian", "Elie"]
    res.render("index", {instructors: instructors})
})
```
Inside of the `res.render` method, the 2nd parameter is an object. What does the key instructors refer to (or where is it used)? What does the value instructors refer to (or where is it used)?

- Fix the broken code:
```js
app.get("awesome",function(req,res){
    res.render("/index")
})
```

- Fix the broken code:
```js
app.get("/",function(req,res){
    res.redirect("index")
})
```

- Given the following code:
```js
app.get("/",function(req,res){
    var instructors = ["Matt", "Ian", "Elie"];
    console.log("These are my instructors!", instructors);
})

app.listen(3000)
```
When a user goes to localhost:3000, what is going to appear in the terminal and what will appear in the browser?

- Why can't we use jQuery in our server code (app.js)?
- Explain method_override
- Explain cookies vs sessions
- Explain module.export

### Mongo

Questions taken from http://www.tutorialspoint.com/mongodb/mongodb_interview_questions.htm

- What are NoSQL databases? What are the different types of NoSQL databases?
- What kind of NoSQL database is MongoDB?
- Which are the most important features of MongoDB?
- What is a Namespace in MongoDB?
- Which languages can be used with MongoDB?
- Compare SQL databases and MongoDB at a high level.
- How is MongoDB better than other SQL databases?
- Does MongoDB support foreign key constraints?
- Does MongoDB support ACID transaction management and locking functionalities?
- How can you achieve primary key - foreign key relationships in MongoDB?
- Does MongoDB need a lot of RAM?
- Does MongoDB pushes the writes to disk immediately or lazily?
- Explain the structure of ObjectID in MongoDB.
- MongoDB uses BSON to represent document structures. True or False?
- If you remove a document from the database, does MongoDB remove it from disk?
- Write out the command to insert a document into a database called school and collection called persons.
- What are Indexes in MongoDB?
- How many indexes does MongoDB create by default for a new collection?
- Can you create an index on an array field in MongoDB? If yes, what happens in this case?
- What is a covered query in MongoDB?
- Why is a covered query important?
- Does MongoDB provide a facility to do text searches? How?
- What happens if an index does not fit into RAM?
- How would you list all the indexes on a particular collection?
- At what interval does MongoDB write updates to the disk?
- How can you achieve transaction and locking in MongoDB?
- What is Aggregation in MongoDB?
- What is Sharding in MongoDB? Explain.
- What is Replication in MongoDB? Explain.
- What are Primary and Secondary Replica sets?
- By default, MongoDB writes and reads data from both primary and secondary replica sets. True or False.
- Why are MongoDB data files large in size?
- When should we embed one document within another in MongoDB?
- Why isn't deploying MongoDB on a 32-bit system preferred?
- What is a Storage Engine in MongoDB
- Which are the two storage engines used by MongoDB?
- What is the role of a profiler in MongoDB? Where does it write all the data?
- How does Journaling work in MongoDB?
- What is the command to check whether you are on the master server or not?
- Can you configure the cache size for MMAPv1? How?
- Can you configure the cache size for WiredTiger? How?
- How does MongoDB provide concurrency?
- How can you isolate your cursors from intervening with the write operations?
- Can one MongoDB operation lock more than one databases? If yes, how?
- How can concurrency affect replica sets primary?
- What is GridFS?
Can you run multiple JavaScript operations in a single mongod instance?
- Which command can be used to provide various information on the query plans used by a MongoDB query?


# [Back to readme](../readme.md)
