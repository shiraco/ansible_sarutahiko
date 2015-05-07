ansible_sarutahiko
====

## Overview

Sarutahiko server setup tool on ubuntu(ec2)

## Environment

* target server
  * OS: Ubuntu 14.04
  * Instance type: t2.micro

## Installation

See http://docs.ansible.com/intro_installation.html

## Usage

### Run playbook from local client

1. run playbook on local client

```
$ ansible-playbook site.yml
```

## Running results

Running result summary
Using Ansible plugin [ansible-profile](https://github.com/jlafon/ansible-profile)

```
PLAY RECAP ********************************************************************
sarutahiko | pip install requirements in 'venv' ----------------------- 947.68s
common | install pyenv's python and rehash ---------------------------- 169.20s
common | apt-get upgrade a server -------------------------------------- 51.41s
common | create swapfile ----------------------------------------------- 18.92s
mongodb | apt-get install mongodb -------------------------------------- 17.32s
common | apt-get install basic pkg ------------------------------------- 14.66s
nginx | apt-get install nginx ------------------------------------------ 12.30s
sarutahiko | git clone sarutahiko-server -------------------------------- 9.76s
supervisor | apt-get install supervisor --------------------------------- 9.51s
nginx | add-apt-repository ppa:nginx/stable ----------------------------- 9.21s
52.68.178.10               : ok=45   changed=37   unreachable=0    failed=0
```
