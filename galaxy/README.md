# Ansible Galaxy

Galaxy is a repository for roles. [Ansible-Galaxy](https://galaxy.ansible.com/)

### Syntax
```
ansible-galaxy [action] [options] arguments
```

### Possible actions:

| action | description |
|--------|-------------|
|delete|removes the rol from galaxy repository|
|import|import the role from github into galaxy|
|info|provides more information of a role
|init|generates tree structure for a new roles
|install|install a role from galaxy repository
|list|list the installed roles|
|login|authenticates into galaxy web|
|remove|removes the rol from the server|
|search|searches galaxy for a certain role|

### Install Roles from requeriments
```
ansible-galaxy install -r requirements.yml
```