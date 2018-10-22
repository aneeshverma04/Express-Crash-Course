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

	