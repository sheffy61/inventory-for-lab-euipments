#This is the Class implemented for users of the inventory

# Person Class #

include("adb.php");
This is the connects to the base adb class to be able to connect to the databas

function get\_id($person\_id)
This is a method to get the information a person with the id.

function search\_by\_name($person\_name)
This method searches for a person with the use of the person name

function add\_person($person\_name, $person\_id,$address, $major)
This method enables you to be able to add a person to the database

function delete\_person($person\_name)
This method enables you to delete a person from the database

function edit\_person($person\_id,$person\_name,$major,$address)
This method enables you edit the information of one person

function view\_one\_person(){
This method makes you view the information or the profile of onne person