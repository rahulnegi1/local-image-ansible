# local-image-ansible
ansible scripts to make up my ubuntu image

## prerequisite 
### ubuntu version 22.04/5.15
    rahul@rahul-VirtualBox:~/ansible$ lsb_release -a
    No LSB modules are available.
    Distributor ID:	Ubuntu
    Description:	Ubuntu 22.04 LTS
    Release:	22.04
    Codename:	jammy
    rahul@rahul-VirtualBox:~/ansible$ uname -r
    5.15.0-30-generic
      
### install ansible
    sudo apt update
    sudo apt install software-properties-common
    sudo apt-add-repository --yes --update ppa:ansible/ansible
    sudo apt install ansible

### run ansible 
    sudo ansible-playbook myimage.yaml 

### current tasks 
    install git 
    if no ssh keys present, generate keys in ~/.ssh folder
    install chrome
