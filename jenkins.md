
Install jenkins in Debian

Conditions( (2018): jdk 8 si > à 8 => may be an error when exetuting jenkins

** Si plusieur java installer changer la version par defaut pour le java Home **

***
sudo update-alternatives --config java
***



1 - ajout repository dans debian
--------------------------------------------

**
Download Jenkins.

Open up a terminal in the download directory.

Run java -jar jenkins.war --httpPort=8080.

Browse to http://localhost:8080.

Follow the instructions to complete the installation.

****

Via apt
****

wget -q -O - https://pkg.jenkins.io/debian/jenkins.io.key | sudo apt-key add -
sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
apt-get update
apt-get install jenkins
