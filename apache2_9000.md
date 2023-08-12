# How to install packages for apache using apt at port 9000  

### Step1: Update Package Lists   

`sudo apt-get update`  

### Step2: Install Apache Packages

`sudo apt-get install apache2`  

### Step3: Configure Apache to Listen on Port 9000

The default configuration of Apache listens on port 80 for regular HTTP traffic. To configure it to listen on port 9000, you need to make changes to its configuration file.

`sudo vi /etc/apache2/ports.conf`

Inside the ports.conf file, add or modify the Listen directive to specify port 9000   

`Listen 9000`  

### Step4: Restart Apache

`sudo systemctl restart apache2`



#### Connect to the Server:

Use the ssh command followed by the username and the IP address or hostname of the server to establish an SSH connection.   
Replace username with your actual username and server_ip with the IP address or hostname of the server:    

`ssh username@server_ip`     


http://your-server-ip:9000/

