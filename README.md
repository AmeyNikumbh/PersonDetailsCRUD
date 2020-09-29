# PersonDetailsCRUD
This application is using H2 database..
After running the project, you can hit the API
http://localhost:8080/h2-console
enter the password = password and click on connect
You can see Person table is created in H2 database.
***************************************************
Below are the API's for this project, hit these API 
in postman 

To add person
http://localhost:8080/add/persondetails

pass the requestbody for example
{
   "firstName" : "John",
   "lastName" : "losner" 
}

To update person details
http://localhost:8080/person/{id}

pass the requestbody for example
{
   "firstName" : "Riya",
   "lastName" : "losner" 
}

To get total persons
http://localhost:8080/person/count

To get all persons from database
http://localhost:8080/person/all
********************************************************




