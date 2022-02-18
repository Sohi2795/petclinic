# Spring PetClinic Sample Application

## Getting Started

   Applications required before starting
   
      1. Xampp
      2. Redis
      3. SpringToolSuite (You can use any prefered tool)
      4. Git
   
   Clone this project by using the below command
      
      git init // if git is not initilized
      git clone https://github.com/Sohi2795/petclinic.git

## Database configuration
   This project uses mysql as a backend db to store and retrive the data. You need to install xampp server https://www.apachefriends.org/download.html inorder to access mysql server locally. Once it is done add the required details(url, username and password) in application.properties inorder to connect the spring app to the mysql.
     
   To fetch the owner list and pet list from the redis cache you need to install the redis from the following link https://redis.com/blog/redis-on-windows-8-1-and-previous-versions/.


You need to start mysql server and redis server before starting the project

You need to add the mysql url, username and password in main class file inorder to load the flyway

You can then access petclinic here: http://localhost:8080/


 ## Resolved Two Bugs in the existing project
 1. Once pet is added to the owner, then if tries to change the details of the owner it will overwrite the existing pet owner id to null. So once sucessfull update of owner details the pet won't be visible to the owner 
 2. Unable to update pet details
