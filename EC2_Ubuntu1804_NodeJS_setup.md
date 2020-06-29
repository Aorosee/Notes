# NodeJS Server under AWS EC2 Ubuntu 18.04 LTS Setup Notes (Including Route 53 DNS)
>While I am learning and developing programs, I searched a lot on Internet. Then I was wondering should I take useful informations out and write them down. However, I know that everything change fast on Internet day after day. I will record the date of my last edits on top of this document. For reader's reference only.</br>

>Verison 1.0.1 </br>
>Last Changes: 06/28/2020 </br>

## GUIDE
**1. Create An Instance on EC2** </br>
**2. Route 53 Setup** </br>
**3. Letsencrypt NPM** </br>
**4. Initialized NodeJS Project** </br>

## Git
**Delete local branch:** </br> `$ git branch -d mybranch`  </br>
**Force delete local branch:** </br> `$ git branch -D mybranch` </br>

## Create An Instance on EC2
* Create an instance. </br>
* Save private.pem key in local. </br>
* Setup security group. </br>
![Security Group Screenshot](https://github.com/Aorosee/Notes/blob/master/src/Images/Security_Group2.png) </br>
* Setup SSH. </br>
![Security Group Screenshot](https://github.com/Aorosee/Notes/blob/master/src/Images/SSH_setup.png) </br>
* Allocate an elastic IP address. </br>

## Route 53 Setup
* Register or transfer a domain into Route53 </br>
* Create a hosted zone </br>
* Create a Record Set </br>
* Resovle domain to Public IPv4 address </br>

## Letsencrypt NPM
* On Ubuntu 18.04 </br>
`$ sudo apt-get update`  </br>
`$ sudo apt-get install software-properties-common`  </br>
`$ sudo add-apt-repository universe`  </br>
`$ sudo add-apt-repository ppa:certbot/certbot`  </br>
`$ sudo apt-get update`  </br>
</br>
`$ sudo apt-get install certbot`  </br>
* IF web server is not cuurently running.
  - `$ sudo certbot certonly --standalone`  </br>
* IF web server is running.
  - `$ sudo certbot certonly --webroot`  </br>

## Initialized NodeJS Project
