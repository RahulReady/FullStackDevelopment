## Backend notes

__node:__ liberating javascript from the browser and onto your computer.
```
// Runs js files on computer where you have to be in a folder that contains the .js file
node filename.js
```
__Node Repl (Read evaluation print loops)__ <br> Can perform JS commands on the console and get results.
<br>
```
// creates a location where you can store many packages aka dependencies.
npm init
// importing packages/ like in pythom
var userDefinedName = require('moduleName');
```
__Express__ - It is to node as JQuery is to Javascript. No need to write redundant/ repetitive code!

__Useful Functions__
```
// gets the path of current folder no matter the type of environment
console.log(__dirname);
```
__Basics of Express__
```
// importing and initializing express (after installing via npm)
const express = require('express');
const app = express();

// once app gets to 'home page', the innput to the call back funct is request and the output is the response.
app.get('/', function(req, res){
  res.send('<h2>Hello!</h2>');
});
```

__Body-parser__
```
// used for parsing web data

// parsing form data
app.use(bodyParser.urlencoded({extended : true}));
```