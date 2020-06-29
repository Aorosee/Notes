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
* 1. Create an instance. </br>
* 2. Setup security group. </br>
![Security Group Screenshot](https://github.com/Aorosee/Notes/blob/master/src/Images/Security_Group.png)
* 3. Setup SSH
