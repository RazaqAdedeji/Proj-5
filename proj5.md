## Project 5 Documentation

### 1. Create and configure two Linux-based virtual servers (EC2 instances in AWS).

![E2C](./images/E2c.png)

### 2. On mysql server Linux Server install MySQL Server software.

![Apt update](./images/sud%20apt%20upda.png)

![install server](./images/install%20mysql%20server.png)

![Enable mysql](./images/systemctl%20enable.png)

![Sudo mysql](./images/sud%20mysql.png)

![Alter user](./images/Alter%20user.png)

### 3. On mysql client Linux Server install MySQL Client software.

![Apt update](./images/sudo%20apt%20upd.png)

![install mysql client](./images/install%20mysql%20client.png)

### 4. By default, both of your EC2 virtual servers are located in the same local virtual network, so they can communicate to each other using local IP addresses. Use mysql server's local IP address to connect from mysql client. MySQL server uses TCP port 3306 by default, so you will have to open it by creating a new entry in ‘Inbound rules’ in ‘mysql server’ Security Groups. For extra security, do not allow all IP addresses to reach your ‘mysql server’ – allow access only to the specific local IP address of your ‘mysql client’.

![E2C TCP](./images/TCP%203306.png)

### 5. You might need to configure MySQL server to allow connections from remote hosts.


'sudo vi /etc/mysql/mysql.conf.d/mysqld.cnf'

### Create User & Database in my mysql and grant access with privilege

![Create command](./images/create%20user%20in%20mysql%20env.png)

### 6. From mysql client Linux Server connect remotely to mysql server Database Engine without using SSH. You must use the mysql utility to perform this action.

![SHow IP add on server](./images/show%20ip%20add.png)

![Connectclient to server](./images/connect%20client%20to%20server.png)

### 7. Check that you have successfully connected to a remote MySQL server and can perform SQL queries:

'Show databases'

![Dispaly db](./images/show%20db.png)