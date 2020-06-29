# NodeJS Server under AWS EC2 Ubuntu 18.04 LTS Setup Notes (Including Route 53 DNS)
>This note is focusing on the details to build a NodeJs Server instance on AWS with friendly domain name.</br>

>Last Changes: 06/28/2020 </br>

## GUIDE
**0. Current Targets/Issues** </br>
**1. Create An Instance on EC2** </br>
**2. Route 53 Setup** </br>
**3. Initialized NodeJS Project** </br>
**4. Port 80 Setup** </br>
**5. Letsencrypt (Port 443 Setup)** </br>
**6. Maintain NodeJS Server** </br>

## Current Targets/Issues
* Redirect to Https from ExpressJS (Helmet?) </br>
* Cert/PryKey file access </br>

## Create An Instance on EC2
* Create an instance. </br>
* Save private.pem key in local. </br>
* Setup security group. </br>
![Security Group Screenshot](https://github.com/Aorosee/Notes/blob/master/src/Images/Security_Group2.png) </br>
* Setup SSH. </br>
![SSH setup Screenshot](https://github.com/Aorosee/Notes/blob/master/src/Images/SSH_setup.png) </br>
* Allocate an elastic IP address. </br>

## Route 53 Setup
* Register or transfer a domain into Route53 </br>
* Create a hosted zone </br>
* Create a Record Set </br>
* Resovle domain to Public IPv4 address </br>

## Initialized NodeJS Project
* Initial npm environment </br>
* Install ExpressJS </br>
* Install Nodemon </br>

## Port 80 Setup
`$ sudo apt-get install libcap2-bin`  </br>
`$ sudo setcap cap_net_bind_service=+ep /usr/bin/node`  </br>
* Search node directory: `$ which node` ('/usr/bin/node') </br>

## Letsencrypt (Port 443 Setup)
* On Ubuntu 18.04 </br>
`$ sudo apt-get update`  </br>
`$ sudo apt-get install software-properties-common`  </br>
`$ sudo add-apt-repository universe`  </br>
`$ sudo add-apt-repository ppa:certbot/certbot`  </br>
`$ sudo apt-get update`  </br>
`$ sudo apt-get install certbot`  </br>
* IF web server is not cuurently running.
  - `$ sudo certbot certonly --standalone`  </br>
![certbot Screenshot](https://github.com/Aorosee/Notes/blob/master/src/Images/Ryore_com_SSL_Certification.png) </br>
* IF web server is running.
  - `$ sudo certbot certonly --webroot`  </br>

## Maintain NodeJS Server
* Start a server: `$ nodemon` OR `$ node app.js`
* Stop/Terminate a server:
  - `$ ps aux | grep node` To check all running process which include keyword node.
  - `$ kill -9 PROCESS_ID` PROCESS_ID is the second column from left side.
