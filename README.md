# Mac Ansible Playbook

This is the playbook I run whenever I setup a new mac, or decide to reinstall my OS.

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
