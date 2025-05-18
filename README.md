# deploy-a-server
Deploy a Server to EC2 (HTML)

This project shows how I deployed a simple static website (HTML) to an AWS EC2 instance using Apache.
Steps I Followed:
	1.	Launched an EC2 Instance
	•	Ubuntu 
	•	Opened port 80 (HTTP) in the security group
	2.	Connected to my EC2 instance via SSH
	3.	Updated and installed Apache
4. i installed nginx
*sudo apt update
*sudo apt install nginx -y
5. i verified nginx was working by using 
*sudo systemctl status nginx
6. cloned the GitHub repository
*git clone https://github.com/audreyeyamike/deploy-a-server.git
*cd deploy-a-server
7. copied my index file to the apache directory
*sudo cp index.html /var/www/html
8. i removed default nginx page
*sudo rm /var/www/html/index.nginx-debian.html
9. restart nginx
*sudo systemctl restart nginx
10. visited my deployed page
