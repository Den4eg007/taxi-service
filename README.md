[![Build Status](https://api.travis-ci.com/den4eg007/taxi-service.svg?branch=master)](https://travis-ci.com/den4eg007/taxi-service)
# Taxi Service
The goal of this project is to create a taxi service with authentication system, custom injector and annotations and all the features that might come in handy while managing the app:
- create new car / manufacturer
- display all drivers
- add driver to the car
- remove driver from car, etc.

## Implementation details and technologies
Project based on 3-layer architecture:
- Presentation layer (controllers)
- Application layer (services)
- Data access layer (DAO)

### Technologies
* Apache Tomcat - version 9.0.46
* MySQL - version 8.0.25
* JDBC
* Servlet
* JSTL
* JSP
* HTML, CSS

## Setup
1. Configure Apache Tomcat
2. Install MySQL and MySQL Workbench
3. Create a schema and all the necessary tables by using the script from resources/init_db.sql in MySQL Workbench
4. In the /util/ConnectionUtil.java change the URL, MYSQL_DRIVER, USERNAME and PASSWORD properties to the ones you specified when installing MySQL or you can use the ones that are already present
5. After starting tomcat go to http://localhost:your port that you specified while configuring tomcat, click on "Register" to add a new driver.

This project is also deployed on heroku: [DEMO](https://taxi-service-product.herokuapp.com/)
