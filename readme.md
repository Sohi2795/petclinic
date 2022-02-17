# Spring PetClinic Sample Application

## Database configuration
   This project uses mysql as a backend db to store and retrive the data. You need to install xampp server https://www.apachefriends.org/download.html inorder to access mysql server locally. Once it is done add the required details(url, username and password) in application.properties inorder to connect the spring app to the mysql.
     
   To fetch the owner list and pet list from the redis cache you need to install the redis from the following link https://redis.com/blog/redis-on-windows-8-1-and-previous-versions/.


You need to start mysql server and redis server before starting the project

You can then access petclinic here: http://localhost:8080/


 ## Resolved Two Bugs in the existing project
   ## 1. Once pet is added to the owner, then if the tries to change the details of the owner it will overwrite the existing pet owner id to null.
   ## 2. Unable to update pet details
