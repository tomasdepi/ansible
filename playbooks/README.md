# Ansible Playbooks

## What's a Playbook
A playbook is a list of plays. A play is minimally a mapping between a set of hosts selected by a host specifier (usually chosen by groups but sometimes by hostname globs) and the tasks which run on those hosts to define the role that those systems will perform. There can be one or many plays in a playbook.

## How to run a Playbook?
```
ansible-plabook -i hosts playbook.yaml
```

## Usuful options and parameters
| Option | Description |
|--------|-------------|
| --syntax-check | Perfoms a syntax validation, it doesn't execute the playbook, just outputs errors if there is someone |
| --list-task | Lists all the tasks |
| --list-hosts | Lists all hosts, that our tasks will provision |
| --step | Before every task, anisble will prompt a question to be sure we want to execute or discard a task |
| --start-at-task='task' | It recevies the name of a task as parameter. Ansible will execute starting from that task and will not execute tasks declared before |
| --forks=10/-f=10 | Amount of parallel tasks |
| -v (vvv) | Increase verbosity |