# Eat the Burger!

*Eat the Burger* is a simple full stack appliacation that allows users to add a burger of their choice, and later devour or delete it.

All user-driven changes - add / devour / delete - are synchronized with a backend MySQL database.

## App Design
[Eat the Burger](https://eat-da-burger-msr.herokuapp.com/) is built on the [MVC](https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93controller) framework

The _model_ utilizes a custom [ORM](https://en.wikipedia.org/wiki/Object-relational_mapping) to provide the backend SQL C-R-U-D functionality, such as Creating (adding) a new burger in the SQL table,  Reading (displaying) all the burger entries from the SQL table, Updating the status of a given burger from 'ready to be eaten' (devoured=false) to 'devoured' (devoured=true), and finally Deleting a given burger from the table.

The _controller_, built with Express.js, handles all the routes and logic. This is where the relevant function provided by the _model_ is invoked based on the path the user selects.

The _view_ is the front-end built with HTML, CSS and jQuery. Dynamic content is rendered using Handlebars.

## Tools/Technologies Used
- Node.js
- Express.js
- MySQL
- NPM libraries - mysql, body-parser, express, express-handlebars
- HTML/CSS
- jQuery/AJAX
- Handlebars