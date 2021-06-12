# Ansible

## Install Ansible

### Centos / Red Hat

```
yum install epel-release
yum install ansible
ansible --version
```

### Ubuntu
```
apt install software-properties-common
apt-add-repository ppa:ansible/ansible
apt update
apt install ansible
```

### Debian
```
echo 'deb http://ppa.launchpad.net/ansible/ansible/ubuntu trusty main' >> /etc/apt/sources.list
apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 93C4A3FD7BB9C367
sudo apt update
sudo apt install ansible 
```

## Cheatsheet

Invoke module:
```
ansible localhost -m ping
```
Invoke module with params:
```
ansible -i hosts server1 -m stat -a "path=/etc/services get_attributes=true"
```
Invoke command:
```
ansible localhost -a "hostname"
```
Specify the user who's gonna try the ssh connection:
```
ansible localhost -u depi -a "hostname"
```

