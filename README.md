# wslhelper
requires ansible and wsl
https://www.digitalocean.com/community/tutorials/how-to-install-and-configure-ansible-on-ubuntu-22-04

also assumes that these are installed
apt-get install nginx
apt-get install mysql-server
apt-get install php8.1-bcmath php8.1-cli php8.1-common php8.1-curl php8.1-gd php8.1-mbstring php8.1-mysql php8.1-opcache php8.1-readline php8.1-soap php8.1-xml php8.1-zip php8.1-fpm

curl -O https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar
chmod +x wp-cli.phar
sudo mv wp-cli.phar /usr/local/bin/wp
https://make.wordpress.org/cli/handbook/guides/installing/


cp config/template config/mysite.json
sudo ansible-playbook localSiteCreate.yaml --extra-vars "@config/mysite.json"
