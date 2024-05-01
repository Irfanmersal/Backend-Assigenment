# Backend-Assigenment
Assume sample data for users &amp; user type in the backend itself, no need to add a database for this. Implement login authentication and JWT authorization and a successful login token should be provided.
Build an application for a library of books. It will have 2 types of users. Admin user and a Regular user.
Implement a /login endpoint:
Assume sample data for users & user type in the backend itself, no need to add a database for this. Implement login authentication and JWT authorization and a successful login token should be provided. 

Implement a /home endpoint that will output a list of books according to the user type:
For regular users, read a file named regularUser.csv that contains some book names and send the book names in the API response.
For admin users, read the file named regularUser.csv and also read the file adminUser.csv and send all the book names in the API response.

Implement a /addBook endpoint
Only admin type of user can access this endpoint
Accept parameters for Book Name, Author & Publication Year in this endpoint
Validate parameters as below:
Book Name & Author should be a string
Publication year should be a number depicting a valid year
If parameters are valid then do the following:
In regularUser.csv file, add this newly added book in the file content 
Calling /home endpoint should now show this newly added book also in the API response along with existing book records

Implement a /deleteBook endpoint
Only admin type of user can access this endpoint
Accept parameter for Book Name in this endpoint
Validate parameters as below:
Book name should be a string and should ignore upper/lower case while matching book name in CSV record
If parameters are valid then do the following:
In regularUser.csv file, delete this book from the file content 
Calling /home endpoint should now show all books except the deleted book in the API response

