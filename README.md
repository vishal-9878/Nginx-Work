# Nginx & Apache Load Balancing
# Dockerized Load Balancing for Sample Backend Application

This project demonstrates how to set up load balancing for a sample backend application running on Docker containers using both NGINX and Apache HTTP Server.

## Prerequisites

- Docker installed on your system
- Basic understanding of Docker and containerization
- Basic knowledge of NGINX and Apache HTTP Server configuration

## Getting Started

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/vishal-9878/Nginx-Work


2. Navigate to the project directory:
   ```bash
   cd your-repo
   
3. Run the sample backend application in Docker containers:
   ```bash
   docker-compose up -d

4. Verify that the containers are running:
   ```bash
   docker ps

5. Setting up NGINX Load Balancer
6. Install NGINX on your system if not already installed:
   ```bash
   sudo apt update
   sudo apt install nginx

7. Configure NGINX as a load balancer by editing the NGINX configuration file (nginx.conf). An example configuration is provided in this repository (nginx/nginx.conf).

8. Restart NGINX to apply the configuration changes:
   ```bash
   sudo systemctl restart nginx
   
9. Access your application through NGINX load balancer.

## Setting up Apache HTTP Server Load Balancer
1. Install Apache HTTP Server if not already installed:
   ```bash
   sudo apt update
   sudo apt install apache2
2. Enable required Apache modules:
   ```bash
   sudo a2enmod proxy proxy_balancer proxy_http

3. Configure Apache HTTP Server as a load balancer by editing the Apache configuration file (load-balancer.conf). An example configuration is provided in this repository (apache/load-balancer.conf).

4. Enable the Apache load balancer configuration:
   ```bash
   sudo a2ensite load-balancer.conf
   
5. Restart Apache to apply the configuration changes:
   ```bash
   sudo systemctl restart apache2
   
## Access your application through Apache HTTP Server load balancer.
