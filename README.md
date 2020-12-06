# Ansible Demo

Do not use this repo for production. It was designed to be used as a demo, not a battle tested live environment.

IP addresses and passwords have been changed to protect the innocent.

## Server Information

These playbooks are meant to be run against CentOS 8 servers.

## Vault Secret

The vault secret for this repo is "password" (no quotes).

## Batteries Not Included

The accompanying Laravel 7 app was not included as similar apps are usually part of job interviews.

Any php app will work if deployed to _/srv/http/public_.

## Local Development

Before running ansible you will need a collection and a role. To install them run:

```sh
ansible-galaxy install -r requirements.yml
```

## First Time Run

The first time you connect to a server you will need to add the ssh fingerprint to your ~/.ssh/known_hosts file. A simple way to do this is using `ssh-keyscan`.

```sh
ssh-keyscan -H [IP_ADDRESS] >> ~/.ssh/known_hosts
```

If you haven't already configured a user to use ssh keys you will need to supply the username (`-u`) and password (`-k`) on the command line. The `-k` flag will prompt you for the ssh password for the root user.

```sh
ansible-playbook -ku root -i hosts -l webserver01 amayer.yml
```
