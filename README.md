# Install Ansible

Centos / Red Hat

```
yum install epel-release
yum install ansible
ansible --version
```

Ubuntu
```
apt install software-properties-common
apt-add-repository ppa:ansible/ansible
apt update
apt install ansible
```

Debian
```
echo 'deb http://ppa.launchpad.net/ansible/ansible/ubuntu trusty main' >> /etc/apt/sources.list
apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 93C4A3FD7BB9C367
sudo apt update
sudo apt install ansible 
```
