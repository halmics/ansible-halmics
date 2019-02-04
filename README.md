# halmics-ansible

## Setup

### Ubuntu Server

```sh
sudo apt-get update && sudo apt-get install -y python2.7 python-simplejson
```

## Usage

e.g.

```sh
ansible-playbook site.yml -i production.inv --ask-pass --ask-become-pass -u [username]
```

or

```sh
ansible-playbook  site.yml -i production.inv --ask-become-pass -u [username] --private-key="~/.ssh/id_rsa"
```
