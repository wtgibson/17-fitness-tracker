# 17 NoSQL: Fitness Tracker

## Summary 

The purpose of the assignment was to create a burger logger with MySQL, Node, Express, Handlebars and a homemade ORM following the MVC design pattern; using Node and MySQL to query and route data in your app, and Handlebars to generate your HTML.

```
Acceptance Criteria

- Application deployed via Heroku
- README.md required
- Application added to personal portfolio page
```

## Application Site

![Site](public/assets/img/burgers-site.png)

## Technologies Used

- HTML - used to create elements on the DOM
- CSS - styles HTML elements on page
- Bootstrap - CSS framework directed at responsive, mobile first front-end web development
- JavaScript - provides dynamic interactivity on HTML documents
- jQuery - easy to use API library simplifying Javascript actions
- Node.js - asynchronous event-driven JavaScript runtime
- Express - Node.js web application server framework, designed for building web applications
- MySQL - open-source relational database management system
- Git - version control system to track changes to source code
- GitHub - hosts repository that can be deployed to GitHub Pages

## Installation & Use

To use the application simply use the deloyed site link below:

https://burgers-wtg.herokuapp.com

## Code Snippet

Below is a block of code in the controller JS file that routes the root index file to the browser.

```js
router.get("/", function(req, res) {
  burger.all(function(data){
    var hbsObject = {
      burgers: data
    };
    console.log(hbsObject);
    res.render("index", hbsObject);
  });
```
[Deployed Site](#)

[GitHub Project Repo](https://github.com/wtgibson/17-fitness-tracker)

## Author Links

![Site](images/william-gibson-jr-photo.jpg)

Will Gibson

[LinkedIn](https://www.linkedin.com/in/wtgibson/)

[GitHub](https://github.com/wtgibson)