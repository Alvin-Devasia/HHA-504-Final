HHA 504 Final

Step 1
Launch the virtual machine
-Microsoft Azure
-UBUNTU server with username and password
-Ports 22(SSH) and 3306(MySQL)
-Create username and password
-Review configs and Create the Virtual Machine

Step 2 
Access the Remote Machine via your Terminal
-Using a terminal, "ssh client@52.154.76.162"  was used to connect to the new VM
-Enter the set password
-Update the UBUNTU server with "sudo apt-get update"
-Install mysql on the virtual machine with "sudo apt install mysql-server mysql-client"
-Enter mysql typing "sudo mysql"

Step 3
Create a new user
-CREATE USER ‘dba'@'%' IDENTIFIED BY ‘ahi2020’;
-THEN CONFIRM: select user from mysql.user;
-GRANT ALL PRIVILEGES ON *.* TO 'dba'@'%' WITH GRANT
OPTION;
-THEN CONFIRM: show grants for dba;
-After the previous steps, Test local user connection by typing "mysql -u dba -p"
-Enter 

Step 4
Create a new database
-Create a new database by typing "Create database e2e;"
-Confirm creation of database by typing "Show databases;"

