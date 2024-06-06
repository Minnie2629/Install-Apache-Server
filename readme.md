#!/bin/bash
# description : Apache server
# author : minnie
# date : 06/04/2024

sudo yum install -y httpd 
sudo systemctl start httpd
sudo systemctl enable httpd
echo "<h1>Deployed via terraform</h1>" | sudo tee /var/www/html/index.html