
# README for Burger Logger MVC App
          
## Description 
              
An application which allows a user to input their favourite burgers, which are stored in two discreet lists - burgers which have been consumed and burgers which the user would like to eat. The app utilises an Model, View, Controller (MVC) structure and uses MySQL, Node, Express, Handlebars and a home-made ORM specific to this application.
        
## Table of Contents
* Title
* Description
* Installation
* Useage
* License
* Contributing
* Tests
* Questions

    
## Installation
To install this application, the user runs the “server.js file in Node (or when deployed uses the app through the html interface). The server establishes the port on 8080 and requires express, which is used to run the server, drawing on the files in the “public directory”. The public directory holds the JS functions (burgers.js) and the CSS. The app is then based around the “Model, View, Controller” structure. The burger.js file is held in the model folder and calls on the ORM which has been constructed for this app. The ORM constructs the databased queries, which are called by the burger.js to create the entries and conduct the three major functions (selectAll, insertOne and updateOne). The “Views” part of the app consists of three handlebars files which provide the front-end templates. Finally, the “Controller” is responsible for creating all of the routes for the server to use, including get, post and put functions for the router. The back-end database is a MySQL database (burgers_db) that is seeded with four initial entries. 

The below directory structure highlights the “MVC” nature of this application:

```
.
├── config
│   ├── connection.js
│   └── orm.js
│ 
├── controllers
│   └── burgers_controller.js
│
├── db
│   ├── schema.sql
│   └── seeds.sql
│
├── models
│   └── burger.js
│ 
├── node_modules
│ 
├── package.json
│
├── public
│   └── assets
│       ├── css
│       │   └── burger_style.css
│       └── img
│           └── burger.png
│   
│
├── server.js
│
└── views
    ├── index.handlebars
    └── layouts
        └── main.handlebars
```

## Usage 
“Eat-Da-Burger” is a restaurant app that lets users input the names of burgers they'd like to eat.  Whenever a user submits a burger's name, the app will display the burger at the top of the page -- waiting to be devoured.  Each burger in the waiting area also has a “Devoured!” button. When the user clicks it, the burger will move below to the section “Burgers that I have already tried/eaten”. The app stores every burger in a database, whether devoured or not. The application requires several node packages: express, MySQL and handlebars.  


## Credits
This was a solo project, however the project relied heavily on Node JS and the packages mentioned above. I sought advice from my class instructors, the Ask BCS instructors and would like to thank Renato for his assistance during our Sunday night tutoring sessions.

## License
MIT

## Badges

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Contributing
Should others wish to contribute to this application, I thank them for their interest and request that they use the standards from at the Contributor Covenant
Note: the [Contributor Covenant](https://www.contributor-covenant.org/) is an industry standard

## Tests
There were no tests developed for this application.

## Questions
Please direct questions to Please direct questions to Please direct questions to Andrewmiddleton1, https://github.com/andrewmiddleton1
