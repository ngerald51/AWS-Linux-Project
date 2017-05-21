# AWS-Linux-Project

# Linux Server Configuration:

Installation of a Linux distribution on a virtual machine and prepare it to host your web application(Item Catalog). It includes installing updates, securing it from a number of attack vectors and installing/configuring web and database servers.

* The EC2 URL is : 'http://ec2-34-200-254-81.compute-1.amazonaws.com/'
* Local IP address: `http://34.200.254.81`
* SSH port- `2200`

* Login with: `ssh -i ~/.ssh/udacity_key.rsa -p 2200 grader@34.200.254.81`

* Generate public Key for udacity_key.rsa :
  * go to .ssh folder of your local machine in which you paste your udacity_key.rsa private key.
  * type this command - `ssh-keygen -y -f udacity_key.rsa` to print the public key .
  * copy and paste this public key in  `/home/grader/.ssh/authorized_keys` so that reviewer can login into grader account .

## Configuration Steps:
### Launch your Virtual Machine with your Udacity account
* Development Environment Information Details:-
  * Public IP Address -  34.200.254.81
  * Private Key - Can't be shared

### Follow the instructions provided to SSH into your server
* `mv ~/Downloads/udacity_key.rsa ~/.ssh/`
* `chmod 600 ~/.ssh/udacity_key.rsa`
* `ssh -i ~/.ssh/udacity_key.rsa root@34.200.254.81`



### Summary of software you installed 
* sudo apt-get update` - command will  update list of packages and their versions on your machine.
* sudo apt-get upgrade` - command will install the packages
* sudo apt-get install libapache2-mod-wsgi` .
* sudo apt-get install apache2
* sudo apt-get install git
* sudo apt-get install python-dev
* sudo apt-get install python-pip
* sudo pip install Flask

* sudo apt-get install python-pip
* pip install httplib2
* pip install requests
* sudo pip install --upgrade oauth2client
* sudo pip install sqlalchemy
* pip install Flask-SQLAlchemy
* sudo pip install flask-seasurf
* sudo apt-get install postgresql postgresql-contrib
* sudo apt install unattended-upgrades
* `sudo apt-get install python-pip`
* `source venv/bin/activate`
* `pip install httplib2`
* `pip install requests`
* `sudo pip install --upgrade oauth2client`
* `sudo pip install sqlalchemy`
* `pip install Flask-SQLAlchemy`
* `sudo pip install flask-seasurf`

### Resource References

**Resources -** [Add User and give permissions](https://www.digitalocean.com/community/tutorials/how-to-add-and-delete-users-on-an-ubuntu-14-04-vps)

**Resources -** [update and upgrade the packages](https://wiki.ubuntu.com/Security/Upgrades

**Resources -** [initial server setup](https://www.digitalocean.com/community/tutorials/initial-server-setup-with-ubuntu-14-04), [udacity course videos](https://classroom.udacity.com/nanodegrees/nd004/parts/00413454014/modules/357367901175461/lessons/4331066009/concepts/48010894750923#)
**Resources -** [UFW](https://help.ubuntu.com/community/UFW)

**Resources -** [timezone to UTC](http://askubuntu.com/questions/138423/how-do-i-change-my-timezone-to-utc-gmt/138442)

**Resources -** [install apache using linux course videos](https://classroom.udacity.com/nanodegrees/nd004/parts/00413454014/modules/357367901175461/lessons/4340119836/concepts/48189486140923#), [install apache](http://blog.udacity.com/2015/03/step-by-step-guide-install-lamp-linux-apache-mysql-python-ubuntu.html) ,[unable to solve host](http://askubuntu.com/questions/59458/error-message-when-i-run-sudo-unable-to-resolve-host-none)

**Resources -** [Install postgresql](https://www.digitalocean.com/community/tutorials/how-to-secure-postgresql-on-an-ubuntu-vps) , [engine configuration](http://docs.sqlalchemy.org/en/rel_1_0/core/engines.html#postgresql)

**Resources -** [Udacity Discussion Forum](https://discussions.udacity.com/t/client-secret-json-not-found-error/34070) , [forum post]( https://discussions.udacity.com/t/how-to-login-to-my-aws-virtual-server-as-new-user-grader/201164/4).

**Resources -** [Udacity Discussion Forum](https://discussions.udacity.com/t/setting-facebook-valid-oauth-redirect-uris/160617) , [Forum post](https://discussions.udacity.com/t/oauth-course-google-sign-in-doesnt-work/15444/2).

**Resources -** [unattended upgrades](https://help.ubuntu.com/12.04/serverguide/automatic-updates.html).

