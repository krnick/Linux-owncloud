# Linux-owncloud


sudo curl https://download.owncloud.org/download/repositories/stable/Ubuntu_16.04/Release.key | sudo apt-key add -


echo 'deb https://download.owncloud.org/download/repositories/stable/Ubuntu_16.04/ /' | sudo tee /etc/apt/sources.list.d/owncloud.list

sudo apt-get update

sudo apt-get install owncloud


sudo systemctl reload apache2


mysql -u root -p

CREATE DATABASE owncloud;

GRANT ALL ON owncloud.* to 'owncloud'@'localhost' IDENTIFIED BY 'password...';

FLUSH PRIVILEGES;

exit



https://server_domain_or_IP/owncloud
