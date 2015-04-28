//start with a class that extends from an adb class with connect and query methods

Manufacturer Class
A class that provides information on manufactures from table with manufacturer\_name, manufacture-id and manufacturer\_address.

include("adb.php"); This method connects to the base adb class to be able to access the database.

function get\_id($manufacturer\_id){
This is a method to get the information of a manufacturer by a given id.

function search\_by\_name($manufacturer\_name){
This method searches for a manufacturer with the use of the person name from the database.

function add\_manufacturer($manufacturer\_name, $manufacturer\_id, $manufacturer\_address){
This method enables you to be able to add a manufacturer details to the database.

function delete\_manufacturer($manufacturer\_name){
This method connects to the database and deletes one record of a manufacturer identified by the name.

function edit\_manufacturer($manufacturer\_id,$manufacturer\_name,$address){
This method enables you edit the information of a manufacturer from the database.

function view\_one\_manufacturer(){
This method allows you to view the information or the profile of a manufacturer from the database.


