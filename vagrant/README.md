
## Vagrant Virtual Machines

Setup one or more Virtual Machines with the required software in an "Infrastructure as Code" way. 
Thanks to Vagrant and Ansible all the process will be completely automated. 
In addition, it's very easy to increase or reduce the number of VM's simply modifying the Vagrantifile.

## Prerequisite steps

VirtualBox, Vagrant and Ansible need to be installed. You can find the installation steps in the official web sites.

#### VirtualBox

https://www.virtualbox.org/

#### Vagrant

https://www.vagrantup.com/

#### Ansible

https://docs.ansible.com/

## And now? How does it work

1) First you need to clone this git repository

2) Next cd into the cloned git directory and check if you can see the <strong>Vagrantfile</strong> and the <strong>master_playbook.yaml</strong> files. The first one is used by Vagrant to setup the VM's. The second, instead, is used by Ansible to run commands and install software on the previously mentioned VM's. Be sure to execute the following commands from inside this folder otherwise they won't work.

3) Finally you need to know a few Vagrant commands to operate with the cluster using the terminal. The most important one are:

- <strong> vagrant up --provision</strong> => spin up the cluster (--provision is used to run Ansible scripts on the VM's, but should be optional).

- <strong> vagrant status </strong> => check the status of the virtual machines.

- <strong> vagrant halt -f </strong> => stop all the VM's.

- <strong> vagrant destroy -f </strong> => stop and destroy all the VM's.

- <strong> vagrant ssh <vm-name> </strong> => ssh into a VM by using its name
  
- <strong> vagrant ssh-config </strong> => info related about the ssh (useful to connect to the VM with plain ssh instead of using vagrant ssh) 

- <strong> vagrant --help </strong> => Vagrant help

