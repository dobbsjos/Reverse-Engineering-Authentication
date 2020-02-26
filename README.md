# Reverse-Engineering-Authentication

The server.js file sets out the npm packages that will be used to direct the sever (express and passport). Express will direct the routes and Passport will allow the user to login to a protected webpage.

The package.json contains the main scripts and the dependences. The main scripts used in this app are test, start and watch. The main dependencies used are bcrypts, express, express-sessions, mysql2, passport, passport-local, and sequalize. Express will be used for the routes. Mysql2 and sequalize will be used for ORM that will give the app prebuilt ways to access the data that is stored in the db. Passport and bcrypts are used to authenticate the user.

The routes folder contains the api and html routes files. The html routes make the call to the server to access infomation. The api routes allow the server to respond.

The public folder contains the main html pages, css, and javascript files. The login.html has the input boxes for loging in. The signup.html has the basic form to allow new user to sign up. The members.html is a protected page that is only accessable by signed in members. The css style sheet adds css to the html pages. The javascript pages contain the code that the html pages need to actually work. The login.js page will be the first page up and will direct correctly logged in members to access the members page. The signup.js will record new members to the db and then allow them to access the login page. The members page just does a get to see which member is signed in.