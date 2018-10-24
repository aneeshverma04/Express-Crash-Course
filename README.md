# Express-Crash-Course

MVC(Model View Controller) framework
Controller = direct traffic , load views
Model = databases
Views = UI

Installation

npm init

WAY 1 ==>
npm install express --save  // save adds this express to package.json
npm install body-parser --save // parse form data etc

WAY 2==>
add dependencies ourselves in package.json
"dependencies":{
	"express":"*", //* for latest version
	"body-parser":"*"
}
npm install to install stated dependencies



Imports
WAY 1 ==>
Use require:
example-> var express = require('express');

WAY 2 ==>
ES6 way
Code must be run through babel
example-> import express from 'express'

* module path ==> to simplify file paths
	Core module= no need to install separately

* index.html always overrides whats in app.js

*** nodemon ..like devtools in spring
Install globally => sudo npm install nodemon -g

$ nodemon app.js

---------------------
Template engines(ejs,pug,jade etc)

EJS=>Embedded javascript
npm install ejs --save

-----------------------
Form validator

Express validator
npm install express-validator --save

----------------
MongoDB

mongo
show dbs
use customerapp
db.createCollection('users')
show collections

db.users.insert([{first_name:'John',last_name:'Doe', email:'jdoe@gmail.com'},{first_name:'beth',last_name:'Smith',email:'bsmith@gmail.com'},{first_name:'Kevin',last_name:'Johnson',email:'kjohnson@gmail.com'}])

db.users.find().pretty()


---mongojs is an ORM..like mongoose
npm install mongojs --save