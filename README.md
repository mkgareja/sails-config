# sails-config(Ubuntu)

##Installation

To install the latest stable release with the command-line tool:
```
sudo npm -g install sails
```
##Creating a New Sails Project

```
sails new testProject
cd testProject
sails lift
```
visit (http://localhost:1337/)

##Environment-specific files (config/env/*)
```
create

config/env/production.js
config/env/development.js
```

##Generating controllers

for create basic controller 

```
$ sails generate controller <controller name> [action names separated by spaces...]
```
with arguments

```
$ sails generate controller user create destroy
```

##Routing

```
  'get /user/:id?': 'UserController.find' // get request with optional argument, it's point find method of User controller
  'post /user': 'UserController.create' // post reuest 
  'put /user/:id?': 'UserController.update' //put request with optional argument
  'delete /user/:id?': 'UserController.destroy' //delete request with optional argument
```

Also sails support [blueprint-api][blueprints].



[blueprints]:<http://sailsjs.org/documentation/reference/blueprint-api>


