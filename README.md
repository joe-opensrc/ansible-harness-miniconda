## An ansible artifact + role to install miniconda and manage conda environments

Installs onto:

 - 

### Dependencies:

Host tested with:

- ansible: v2.13.13
- python:  v3.11.5+

### Steps to prepare:

```
git clone --recurse-submodules https://github.com/joe-opensrc/ansible-harness-miniconda
cd ansible-harness-miniconda 
ansible-playbook -i hosts miniconda.yml --limit <docker-container-name>
```

