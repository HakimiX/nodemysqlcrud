# NodeJS - ExpressJS - MySQL
## Crud Application

### Commands

**Create the project**

```javascript
mkdir app-name
```
```javascript
cd app-name
```

Initialize project
```javascript
npm init
```

**Install required modules**
* express: used to create handle routing and process requests from the client.
* express-fileupload: Simple express file upload middleware that wraps around busboy.
* body-parser: used to parse incoming request from the client.
* mysql: Node JS driver for MySQL.
* ejs: templating engine to render html pages for the app.
* req-flash: used to send flash messages to the view
* nodemon: Installed globally. It is used to watch for changes to files and automatically restart the server.

```javascript
npm install express express-fileupload body-parser mysql ejs req-flash --save
```
```javascript
npm nodemon -g
```


**Create the database** 

```javascript
CREATE DATABASE database-name;
CREATE TABLE IF NOT EXISTS `players` (
  `id` int(5) NOT NULL AUTO_INCREMENT,
  `first_name` varchar(255) NOT NULL,
  `last_name` varchar(255) NOT NULL,
  `position` varchar(255) NOT NULL,
  `number` int(11) NOT NULL,
  `image` varchar(255) NOT NULL,
  `user_name` varchar(20) NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB  DEFAULT CHARSET=latin1 AUTO_INCREMENT=1;
```




