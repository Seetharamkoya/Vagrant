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

