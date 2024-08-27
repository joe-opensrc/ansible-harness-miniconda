## An ansible artifact + role to install miniconda and manage conda environments

Installs onto:

 - rockylinux9 (docker):
    e.g.
      ```
        docker build -f testenv/Dockerfile -t repo/rocky9:miniconda .
        docker run --rm --name miniconda -it repo/rocky9:miniconda
      ```


### Dependencies:

Host tested with:

- ansible: v2.13.13
- python:  v3.11.5+

### Steps to prepare:

```
git clone --recurse-submodules https://github.com/joe-opensrc/ansible-harness-miniconda
cd ansible-harness-miniconda
ansible-playbook -i hosts miniconda.yml --limit miniconda
```

