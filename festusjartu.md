this is a wiki page for my lab.php and login.php
Festus Emmanuel Jartu
Wiki Page
#Lab.php class reference.
Lab class
A class to encapsulate all the lab functions.
Fields
$str\_query
Handles the query information writing of the query.
Methods
adb()
Constructor method
Add\_lab($lab\_name, $lab\_id)
A method to add a lab to the system it returns whether the result was added or not. The method takes in two parameter the lab\_id and the user\_name
search\_by\_name ($lab\_name)
The method takes in the name of the lab it wants to look for and search through the database. The method then returns the result from the search

delete\_lab ($lab\_name)
The method takes in the name of the lab it wants to delete and removes it from database. The method then returns the result after deleting.
update\_lab ($lab\_name, lab\_id)
The method takes in the lab id and name of the lab it wants to update and update it in database. The method then returns the result after update.
Class login
Fields
Object
Gets the user name entered from the document via the id
Object1
Gets the password entered by the user via the document id
$link
It is a database connection reference. The method connect() will store reference in this field
$str\_query
Description of the query exactly the command that is to be sent to the database it returns a result.
Methods
confirmUser
It declares two variables objects and tries to verify the user name against that in the database and likewise the password. When this confirmed the user gains access to the system.

adb class
A class to interface with mysql. It encapsulates mysql php functions.
Fields
$str\_error
Describes error page
$error
Error code from the last error
$link
Database connection reference. connect() method stores the connection reference in this field.
$er\_code\_prefix
Prefix for generating error codes
result
Stores the reference to the dataset after a query is executed successfully by query() method
Methods
adb()
Constructor method
connect()
Connects to mysql and selects database Returns true if connected else false
query($str\_sql)
Runs query on existing db connection. If there is no connection it creates new connection. Returns true if query is successful, else false. The dataset reference is stored in $result.
fetch()
Returns on row from the current data set as associated array. If there is an error it returns false.
get\_num\_rows()
Returns the number of rows in the current dataset.
get\_insert\_id()
Returns an auto increment id from the last insert query executed using the open connection.



