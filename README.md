# ansible-enpass-io
installs [enpass](https://www.enpass.io/) on debian or ubuntu


## example

```
#! /usr/bin/ansible-playbook
---
# run it with
#           ansible-playbook enpass-io.yml
#        or ./packer-io.yml
#                        Thorsten Strusch 2017-07-13
####################################################
- hosts: localhost
  become: yes
  gather_facts: true

  environment:
    http_proxy: http://proxy:3128/
    https_proxy: http://proxy:3128/

  roles:
    - ThorstenS-linux.enpass-io

```
