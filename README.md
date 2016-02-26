# Mac Management Ansible Playbook

This repository is based off of work by
[Jeff Geerling](https://github.com/geerlingguy).  See the source repository
[here](https://github.com/geerlingguy/mac-dev-playbook).

This playbook manages my Mac setup using Ansible.  This playbook is tested on a
Vagrant VM, available [here](https://github.com/AndrewDryga/vagrant-box-osx).

This is a work in progress.  It mostly serves to allow me to reliably and
quickly setup a new Mac for work and fun.

## Installation

1. `xcode-select --install`
2. `sudo easy_install pip`
2. `sudo pip install ansible --quiet`
3. `sudo mkdir /etc/ansible`
4. `sudo chown $(whoami) /etc/ansible`
5. `git clone https://github.com/supertylerc/mac-workstation && cd $_`
6. `ansible-galaxy install -r requirements.txt`
7. `ansible-playbook main.yml -i inventory --ask-sudo-pass`

## Roadmap

* Secrets vault
* Username as a variable
* Full `vim` setup

## Author

[Tyler Christiansen](http://blog.tylerc.me), 2016
[Jeff Geerling](http://jeffgeerling.com/), 2014
Originally inspired by [MWGriffin/ansible-playbooks](https://github.com/MWGriffin/ansible-playbooks)
