# ansible-halmics

## Setup

### Ubuntu Server

```sh
sudo apt-get update && sudo apt-get install -y python2.7 python-simplejson
```

### Host Machine

```sh
ansible-galaxy install -r requirements.yml
```

## Usage

e.g.

```sh
ansible-playbook site.yml -i production.inv --ask-pass --ask-become-pass -u [username] --ask-vault-pass
```

or

```sh
ansible-playbook  site.yml -i production.inv --ask-become-pass -u [username] --private-key="~/.ssh/id_rsa" --ask-vault-pass
```
