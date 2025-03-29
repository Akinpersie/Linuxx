## LAMP STACK (Lab Guide)
### Step 1 — Installing Apache and Updating the Firewall
- Update the package manager cache:
   
    >   sudo apt update

![screenshot-1](lampstacksudoaptupdate.JPG)

- Install Apache:

    >   sudo apt install apache2

    ![screenshot-2](installapache2.JPG)

- Allow HTTP traffic through the firewall:
    
    >   sudo ufw allow in "Apache"

![screenshot-3](httpallow.JPG)

### Step 2 — Installing MySQL
-   Install MySQL:

    >   sudo apt install mysql-server

![screenshot-4](mysql.JPG)

- Connect to MySQL as the root user:

    >   sudo mysql

![screenshot-5](mysqlroot.JPG)

- Change root user's authentication method to mysql_native_password (for compatibility with some PHP versions):

    >   ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';

![screenshot-6](changeroot.JPG)

- Exit the MySQL console:

    >   exit

    ![screenshot-7](mysqlexit.JPG)

- Run the MySQL security script:

    >   sudo mysql_secure_installation

![screenshot-8](mysqlsecurityscript.JPG)

