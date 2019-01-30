### Linux Server Configuration
Project for the Udacity Full Stack Web Development Nanodegree.

#### Introduction
This project hosts the Item Catalog web app on a Linux web server powered by Amazon Web Services.

#### SSH Instructions
Log in to SSH using credentials `grader@100.27.38.183` on port 2200 and the key provided.

#### Web Location
Access the wep application at https://shybull.net.

#### Software Used
* Amazon Lightsail running Ubuntu Linux
* Apache2 and mod_wsgi package
* Python 3 and Flask
* SQLAlchemy
* Let's Encrypt Certbot for https

### Configuration Changes
* All installed packages updated
* SSH changed to port 2200
* UFW set to only allow incoming connections for SSH port 2200, HTTP port 80, HTTPS port 443, and NTP port 123.
* Remote login disabled for `root`
* Users required to authenticate with RSA key
* `grader` user created with sudo permissions and SSH key pair
* Timezone changed to UTC
* Apache configured to server Item Catalog application as WSGI app

#### Resources Used
* Udacity Deploying to Linux Servers course content
* Previous Item Catalog project
* Student Hub feedback
* Stack Overflow for diagnosing errors
