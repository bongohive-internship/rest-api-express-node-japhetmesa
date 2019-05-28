# node-api-with-express
After interacting with bare Node JS, you will be introduced to writing restful APIs in Node JS with Express package.

# Getting Started

To get up and running with Express JS, you will need to install this package. With Node JS packages can be added with tools eaither npm (Node Package Manager) or yarn. In this cause we will use npm. Keep in mind that when you install node, it will also install npm which can readily be used.

Learn more on how to use Node npm on this link and any other usefull link you may find on the Internet 
- https://www.w3schools.com/nodejs/nodejs_npm.asp

Learn how to install a package with npm on the following link or any other useful materials on the Internet.
- https://docs.npmjs.com/downloading-and-installing-packages-locally

# Jumping into code

In this repository, initialize and install express package with npm by doing the following;
- open your terminal in this croned repository
and answer the default questions which will be asked when initializing npm
```bash
 node-api-with-express$ npm init
 ```
 Press enter for most of the questions and answer the following following on some
  - Author add your name
  - license add MIT
  - Entry script add index.js
npm will finish to initialize and will create a file called package.json and a folder called node_modules were all our application dependancies packages are stored by npm.

- Express environment read https://www.tutorialspoint.com/expressjs/expressjs_environment.htm

After initializing the npm package manager on your project, you can now start installing application dependancy packages.

To begin with 
- Create a folder called src in this repository.
- cd into the src folder
- In the folder src, create a file called index.js
- install express package. Check this link for further read https://expressjs.com/en/starter/installing.html
```bash
  $npm install express --save
```
# using express

open index.js file in your code editor, vscode or atom
add the following lines of code to test express api routes

index.js
``` javascript
const express = require('express')
const app = express();

app.get('/', function(req,res){
   
    res.send('Express says hello').end();
    
})

app.listen(3000, function(){
  console.log('Server started and listening on port 3000')
})

```

Save this file and open a terminal in the directory were index.js file is.

From the previous course (setting up node js environment) , you learned on how to start a Node JS server.

So, start your Node JS server by running index.js

In the other course( working with postman), you learned how to mock api, so open postman and enter the url

Mocking created index.js route 
 - http://localhost:3000/

To mock our server. You should see the output "Express says hello". Keep in mind that the created route is a get route. learn more on restful APIs on this link and conduct an assignment

Understanding REST read 
  - https://www.smashingmagazine.com/2018/01/understanding-using-rest-api/
  -  https://medium.com/extend/what-is-rest-a-simple-explanation-for-beginners-part-1-introduction-b4a072f8740f
  
Express available route read 
   - https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction
   - https://www.tutorialspoint.com/expressjs/expressjs_hello_world.htm
   - https://www.tutorialspoint.com/expressjs/expressjs_routing.htm
   - https://www.tutorialspoint.com/expressjs/expressjs_http_methods.htm
   - https://www.tutorialspoint.com/expressjs/expressjs_url_building.htm
   - https://www.tutorialspoint.com/expressjs/expressjs_url_building.htm
   
 # Assignment
 
Read on express from the above provided links, practice and do this assignment.
create the following end-points that return the following. In the src folder create a file called testExpress.js and add all the end points that yoiu will create.
 
 - create an array called provinces of size 10 for all the provinces in Zambia. This array should be accessed by all the                routes that you will create.
 
 - create a json array called countries with 10 objects having fields country name, country capital city and the type of people who live in that country.
 
 - Create a Get Express API route ('/country/provinces') that return all the contents of the provinces array.
 - Create another GET Express API route ('/countries') that will return the contents of the countries json array.
 - Create a POST Express API route ('/countries/provinces') that adds a province to the provinces array
 - Create a POST Express API route ('/countries') that adds a country json object with all the fields to countries json array object.
 
 - Create a DELETE Express API route ('/delete/province') that deletes a province that is sent from the provinces array and returns the deleted province.
 
 - Create a DELETE Express API route ('/delete/country') that deletes a country that has be sent from the countries json array object and returns the deleted country to the user.
 
 - Create a PUT Express API ('/countries/edit') that returns the message "Iam tired man, I think I will edit this country nameOfCountryTOEdit later." to the user.
 
                          USE POSTMAN TO TEST YOUR ROUTE END POINTS
 
 
     Submit this assignment by commiting this repository with all the files index.js and testExpress.js
 
 
 




















