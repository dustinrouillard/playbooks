# Mac Ansible Playbook

This is the playbook I run whenever I setup a new mac, or decide to reinstall my OS.

## Installation

Running this playbook is reletively simple, just have to install ansible and homebrew.

- Install homebrew \
  `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

- Install ansible \
  `brew install ansible`

- Clone this repository \
  `git clone https://github.com/dustinrouillard/playbooks -b mac`

- Install ansible requirements \
  `ansible-galaxy install -r requirements.yml`

- cd into the cloned directory and run playbook \
  `ansible-playbook config.yml -K`

## Tasks

- Installs all the appstore apps I normally use
- Installs all brew and brew cask packages
- Configures all pmset values on my mac
- Installs any .pkg files from urls
- Removes default items and adds perferred items to the dock
- Installs node using fnm and node version 16
- Clones and installs my [dotfiles](https://github.com/dustinrouillard/dotfiles)

## Collections/Roles

- [osx-command-line-tools by elliotweiser](https://github.com/elliotweiser/ansible-osx-command-line-tools)
- [ansible-collection-mac by geerlingguy](https://github.com/geerlingguy/ansible-collection-mac)
- [ansible-role-dotfiles by geerlingguy](https://github.com/geerlingguy/ansible-role-dotfiles)
- [ansible-role-macdock by fubarhouse](https://github.com/fubarhouse/ansible-role-macdock)
