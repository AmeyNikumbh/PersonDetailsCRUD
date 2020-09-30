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
   "lastName" : "losner",
   "addressList": [
   {	"street": "s1",
         "city": "c1",
         "state": "st1",
         "postalCode": "pc1"
   },
   {	"street": "s2",
         "city": "c2",
         "state": "st2",
         "postalCode": "pc2"
   }
   ]      

}

To update person details
http://localhost:8080/person/{pId}/{aId}

pass the requestbody for example
{
    "personId":1,
   "firstName" : "Kiya",
   "lastName" : "losner" ,
      "addressList": [
   {	"addressId":1,
       "street": "s1",
         "city": "c1",
         "state": "st1",
         "postalCode": "pc1"
   },
   {	"street": "s2",
         "city": "c2",
         "state": "st2",
         "postalCode": "pc2"
   }
   ]      

}

To get total persons
http://localhost:8080/person/count

To get all persons from database
http://localhost:8080/person/all

To delete person details
/remove/person/{personId}/{addressId}
********************************************************




