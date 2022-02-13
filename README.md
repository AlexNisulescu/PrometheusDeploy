# Ansible script for installing and configuring Prometheus

## Table of contents
  * [Index](#index)
  * [Introduction](#introduction)
  * [Requirements](#requirements)
  * [How to use it](#how-to-use-it)
  * [Contributors](#contributors)


## Introduction
This repo was created from the need to repeatedly install Prometheus on all sort of hosts
    

## Requirements

Ansible - minimum version: 2.11

You will also need to modify both files in inventory/ : hosts and passwords with your specific addresses and credentials

I recommend encrypting the passwords file using:

    ansible-vault encrypt inventory/passwords

In the role file you will need to go to the /vars/main.yml file and specify the version of prometheus you want to install. Be very carefull when choosing it and keep in mind the os and arhitecture.

## How to use it
Run it with:

    ansible-playbook -i inventory/ main.yml

If you've encrypted the passwords file using the vault command you need to add to the previous command "--ask-vault-password"

Now you have to:

    Sit back and enjoy

## Contributors
    Creator: Alexandru Nișulescu
    Contact: alex.nisulescu1998@gmail.com
    Linkedin: https://www.linkedin.com/in/alex-nisulescu-45822b178/
