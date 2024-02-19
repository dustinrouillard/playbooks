# Arch Ansible Playbook

This is the playbook I run whenever I setup a new arch box, or decide to reinstall my OS.

## Installation

Running this playbook is reletively simple, just have to install ansible.

- Install ansible and git \
  `pacman -S ansible git`

- Clone this repository \
  `git clone https://github.com/dustinrouillard/playbooks -b arch`

- Install ansible requirements \
  `ansible-galaxy install -r requirements.yml`

- cd into the cloned directory and run playbook \
  `ansible-playbook config.yml -K`

## Tasks

- Installs all the packages we need from pacman and the aur
- Installs kitty terminal and configures it
- Installs zsh and oh-my-zsh and switches main shell
- Installs node using fnm and node version 20
- Clones and installs my [dotfiles](https://github.com/dustinrouillard/dotfiles/tree/arch)

## Collections/Roles

- [ansible-role-dotfiles by geerlingguy](https://github.com/geerlingguy/ansible-role-dotfiles)
- [ansible-fnm by hurricanehrndz](https://github.com/hurricanehrndz/ansible-fnm)
- [ansible-aur by kewlfft](https://github.com/kewlfft/ansible-aur)