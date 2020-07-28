# Reverse-Engineering-Code
## Description:
  This app allows user to sign up for account, log into their account and log out from their account Securely.
## Technologies Used:
* BCRYPTJS
* Express
* MYSQL-2
* PASSPORT
* SEQUELIZE
## Getting Started With App:
  To begin using this app, please clone this repository into your local storage. Once this is complete, please follow these steps;
* create a mysql db called "passport_demo". 
* go into the config file, open config.js and insert your personal data ie username, password etc 
* open terminal in current repo and run "npm i" to install all node packages 
* while in terminal, run "node server.js" and you will successfully connect to server 
* open browser and put "http://localhost:8080" in search bar 
* enjoy using the app!
## Files Explained:
### CONFIG:
#### middleware:
* isAuthenticated.js - restricts routes that user is not allowed to visit if not logged in. if user is logged in, it continues with request.
#### Config.json:
   Connection configuration to connect to server.
#### Passport.js:
    Contains javascript logic that tells passport we want to log in with an email address and password.
### MODELS:
#### index.js:
   connects to database and imports users log in data.
#### user.js:
   connects to database and defines the data present in database. Requires bcrypt for password hashing.
### PUBLIC:
   Contains html,css,js front end files.
### ROUTES:
#### api-route:
   contains routes for signing in, logging out and getting users specific data to be displayed client side.
#### html-routes.js:
   routes that check whether user is signed in, whether user already has account etc and sends them to the correct html page.
### Package.json:
   contains all package info, node modules used, version info etc
### Server.js:
  requires packages, sets up PORT, creates express and middleware, creates routes and syncs database ,logs message in terminal on successful connection to server.




