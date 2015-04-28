wiki page for the login.php, inventory.php and adb.php

Kinyari Lydia Kemuma

Inventory class
#login.php class reference
Fields
$str\_query
Stores	the SQL statements for each of the requests
Methods
get\_equipment($id)
Takes in $id as a parameter and returns the details of the equipment corresponding to that id.
search\_by\_name($equipment\_name)
Takes $equipment\_name as parameter and returns the details of the equipment with the corresponding name
add\_equipment($equipment\_name, $description,$price, $manufacturer\_id,$equipment\_id)
Takes in the features of an equipment as parameters and inserts the details into the database as one equipment. It returns the whether the equipment was successfully added or not.
delete\_person($equipment\_name)
Takes as parameter the name of an equipment and deletes it from the database
edit\_equipment($equipment\_id,$equipment\_name,$description,$price)
Takes as parameters the id of an equipment and the new details of the equipment and updates the database


login class
#login.php class reference
A class to authenticate users by interfacing with MySQL
Fields
Var obj
Stores	the username input by the user
Var obj1
Stores	the password input by the user
Methods
Confirm user()
Gets input from the user and compares it with the actual username and password before allowing the user to access the home.php

adb class
#adb.php class reference
A class to allow connection to the database
Fields
$str\_error
Stores the error of the last operation
$error
Stores the error code of the last operation
$link
Stores the database connection reference of the last operation
$er\_code\_prefix
Stores the prefix for generating the codes
$result
Stores the reference to the dataset after a query is executed successfully by query() method
Methods
adb()
Constructor of the class
connect()
Connects to MySQL and selects database Returns true if connected else false
query($str\_sql)
Connects to MySQL and selects database Returns true if connected else false
query($str\_sql)
Runs query on existing db connection. If there is no connection it creates new connection. Returns true if query is successful, else false. The dataset reference is stored in $result.
fetch()
Returns on row from the current data set as associated array. If there is an error it returns false.
get\_num\_rows()
Returns the number of rows in the current dataset.
get\_insert\_id()
Returns an auto increment id from the last insert query executed using the open connection.
log\_error($level, $code, $msg, $mysql\_msg = "NONE")
Logs error or success message by calling log\_msg function. It generates error code ($error$) and error description ($str\_error).