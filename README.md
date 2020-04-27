# Drupal-MySQL

                                 

   # **IIEC Docker Project using drupal and mysql**
This is a multicontainer docker application using drupal and mysql.

## **What is Drupal**

Drupal is a free and open-source content-management framework written in PHP and distributed under the GNU General Public License. It is used as a back-end framework for at least 2.1% of all Web sites worldwide ranging from personal blogs to corporate, political, and government sites including WhiteHouse.gov and data.gov.uk. It is also used for knowledge management and business collaboration.

## **What is MySQL**

MySQL is the world's most popular open source database. With its proven performance, reliability and ease-of-use, MySQL has become the leading database choice for web-based applications, covering the entire range from personal projects and websites, via e-commerce and information services, all the way to high profile web properties including Facebook, Twitter, YouTube, Yahoo! and many more.

 ### Steps to create this multicontainer application. ###

 ### 1  Prerequisites ###
 - This project is completely done on RHEL(Red Hat Enterprise Linux).
 - Install docker on the os using the cmd `yum install docker`.
 - Install docker-compose using the below cmd:
 
  ` curl –L"https://github.com/docker/compose/releases/download/1.25.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose `


 ### 2  Start the Docker Service ###
 -  Use `systemctl start docker` to start Docker Service.
   
 ### 3  Download the required images: ###
 - Pull MySQL Image: 
 
    Use `docker pull mysql:5.7` to download the mysql version 5.7 image to use as a database server.
 - Pull Drupal Image: 
 
    Use `docker pull drupal:8-apache` to download the drupal Image in which apache server is preconfigured.
    
   ![alt text](https://github.com/anandhukrishna1998/Drupal-MySQL1/blob/master/screenshot/docker%20images.PNG?raw=true)
 ### 4 Docker-Compose ###

 -	 Create a docker-compose file with yml extension using `vim docker-compose.yml`
 -	 The yml file is
 
 ![alt text](https://github.com/anandhukrishna1998/Drupal-MySQL/blob/master/screenshot/compose%20yml.PNG?raw=true)
      

### 5 start Docker-compose: ###
 -	Use `docker-compose up -d` to start the docker-compose service in detach mode.


 ![alt text](https://github.com/anandhukrishna1998/Drupal-MySQL1/blob/master/screenshot/compose%20up.PNG?raw=true)
 
 
### 6 Start the Drupal Service ###
 - Open the web browser and type the ip address with port number. In my case it is 192.168.122.1:8080. 
  
  ![alt text](https://github.com/anandhukrishna1998/Drupal-MySQL1/blob/master/screenshot/duplar.PNG?raw=true)

### 7 stop the docker-compose ###
 -	Use` docker-compose stop` to stop the docker-compose service.
 
   ![alt text](https://github.com/anandhukrishna1998/Drupal-MySQL1/blob/master/screenshot/compose%20stop.PNG?raw=true)

 ## References:  ##
 ### To learn docker-container technology from scratch. ###
 
 Youtube link (https://www.youtube.com/playlist?list=PLAi9X1uG6jZ30QGz7FZ55A27jPeY8EwkE)
 


