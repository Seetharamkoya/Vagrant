## Vagrant VM'S
VM with Vagrant Boxes from the vagrant cloud
## Commands
1. Create a Directory with the Any folder "VAGRANT" and also creat a file for vagrant boxes from the cloud using git bash.
3. Vagrant init "Vagrant box name from the cloud" 
4. (It will create the a vagrant file in the folder)
5. vagrant up
6. (It will download the VM into virtual Box and starts running.)
7. vagrant ssh
8. (It will ssh into VM(virtual machine)
9. we can check the "version" and user..
10. vagrant halt 
11. (To close the VM completely)
12. agrant destroy
13. (to delete the VM)

## To connect the public network with VM
Usually, NAT connection is shared with the VM from the Virtual Box. So, to enable to public network "router/wifi -ip" to the VM we need to enable "Bridge connection" to get public IP.
This can be done in the "Editing the Vagrant file of the VM" using Notepad(seting the  config.vm.network "public_network"). \
To save the chanes with the runningVM using the "vagrant reload"(command) \

![Screenshot (255)](https://user-images.githubusercontent.com/38424194/149036114-e2ce70af-bb88-4e19-87ae-09685f0fbcc8.png)

### To install apache2, nodejs and MongoDB in Ubuntu
1. Sudo apt update\
2. create a user and password for the and enable "passwordauthentation yes" in vi /etc/ssh/sshd_config \
3. edit the "sudoers" and give 744 previlages to the user to install.
4. apt install apache2 -y
5. systemctl status apache2
6. systemctl start apache2
7. systemctl enable apache2
8. apt install firewall* -y
9. systemctl status firewalld
10. systemctl start firewalld
11. systemctl enable firewalld
12. firewall-cmd --zone=public --add-port=8080/tcp --permanent
13. firewall-cmd --zone=public --add-service=http --permanent
14. firewall-cmd --reload
15. firewall-cmd --list-all
16. We can acess/validate the the "apche2 webserver" in the browser.
17. ## Nodejs installation
18. We can install in [Node js](https://linuxize.com/post/how-to-install-node-js-on-ubuntu-20-04/) 3 ways.
