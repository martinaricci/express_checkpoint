# Node/Express Test

### Question 1

What is `module.exports` and why do we use it?


The module.exports is a special object which is included in every JS file in the Node.js application by default. module is a variable that represents current module and exports is an object that will be exposed as a module. So, whatever you assign to module.exports or exports, will be exposed as a module. We use it to import code into our application. 

### Question 2

Write one Express route for each of the four CRUD actions.

Then, make each route respond with a one-word string containing the RESTful action that would most likely be associated with this route.

```js
var express = require("express")
var app = express()

app.get('/', (req, res) => {
    res.send('Hello world')
})

app.post('/about-me', (req, res) => {
    res.send('create your page')
})

app.patch('/about-me/:id', (req, res) => {
    res.send('update your details')
})

app.delete('/about-me/:id', (req, res) => {
    res.send('delete some of your infos')
})

```

### Question 3

Describe the differences between Express and Rails as backend frameworks.

EXPRESS: 
    - Nice routing,
    - Better performance, Express is being up to 20 times faster than Rails for certain scenarios, 
    - Using only 3 servers instead of 30. 
    - Express is Javascript and it's a driven architecture which makes it an awesome fit for mobile apps, chatting apps, or any apps that use rest services as a backend and it is able to handle asynchronous requests as well. 
    - Full stack. From HTTP server to templating engine, Node.JS-Express is the whole package.
    - Best for fast single page app or highly interactive apps.
    - Package management: dependencies are installed locally rather than globally. 

 RAILS:
    - Havier and slower than NodeJs,
    - Best for robust web app, 
    - Ruby is very powerful and expressive. It's easy to express application logic in an intuitive way. If you open up someone else's Rails application, you already know how it works. This is why Rails is popular when you need to work with a large team or when you need to be able to hand off your project to someone else after you build it.
    - Database migrations are really helpful and can't be underestimated.
    - Large stack frames. The fact that Rails has so many layers of abstraction makes debugging a pain. If a database call fails, the error message isn't informative. 


### Question 4

What do the following lines of code do?

```js
var bodyParser = require("body-parser")
app.use(bodyParser.json())
app.use(bodyParser.urlencoded({extended: true}))
```
1. var bodyParser = require("body-parser")
    - body-parser extract the entire body portion of an     incoming request stream and exposes it on req.body.

2. app.use(bodyParser.json())
    - returns middleware that parses json

3. app.use(bodyParser.urlencoded({extended: true}))
    - returns middleware that parses encoded data

### Question 5

For this exercise you will be creating an es6 BankAccount class.

It will have the following properties...
* `type` (e.g., "checking"), which should be determined by some input
* `balance`, which should start out as `0`

It should have the following methods...
* `withdraw`, which should decrease the balance by some input
* `deposit`, which should increase the balance by some input
* `showBalance`, which should print the balance in the bank to the console.

The `BankAccount` class has a `transactionHistory` property which keeps track of the withdrawals and deposits made to the account.
* Make sure to indicate whether the transaction increased or decreased the amount of money in the bank.

```text
Your answer...
```

Create an instance of the BankAccount class

```text
Your answer...
```
