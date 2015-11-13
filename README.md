TensorFlow_Study
====

## Overview

Setup deeplearning tool chainer development environment on ubuntu(ec2) GPU instance

## Environment

* target server
  * OS: Ubuntu 14.04
  * Instance type: g2.2xlarge

## Installation

See http://docs.ansible.com/intro_installation.html

## Usage

### SSH setting on local client

1. copy hosts from hosts.sample
```
$ cp hosts.sample hosts
```
2. edit hosts to ssh target server
```
$ vim hosts
```

```text:hosts
[development]
xx.xx.xx.xx ansible_connection=ssh ansible_ssh_user=ubuntu ansible_ssh_private_key_file=~/.ssh/hoge.pem
```

* xx.xx.xx.xx: Your EC2 IP Address
* hoge.pem: Your pem file name

### Run playbook from local client

1. run playbook on local client

```
$ ansible-playbook site.yml
```

## Running results

Running result summary
Using Ansible plugin [ansible-profile](https://github.com/jlafon/ansible-profile)

```

```

## References

* http://chainer.org/

## Lisence

This software is released under the MIT License, see LICENSE.
