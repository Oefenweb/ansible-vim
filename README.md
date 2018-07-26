## vim

[![Build Status](https://travis-ci.org/Oefenweb/ansible-vim.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-vim) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-vim-blue.svg)](https://galaxy.ansible.com/Oefenweb/vim)

Set up vim in Debian-like systems.

#### Requirements

None

#### Variables

* `vim_vimrc_destinations`: [default: `{skell: dest: /etc/skel, current: dest: "{{ ansible_env.HOME }}"}`]: Destinations to copy the vimrc file to
* `vim_vimrc_destinations.key`: The identifier of the file (e.g. `skel`)
* `vim_vimrc_destinations.key.dest`: The remote path of the file to copy (e.g. `/etc/skel`)
* `vim_vimrc_destinations.key.owner`: The name of the user that should own the file (optional, default `root`)
* `vim_vimrc_destinations.key.group`: The name of the group that should own the file (optional, default `owner`, then `root`)
* `vim_vimrc_destinations.key.mode`: The mode of the file, such as 0644 (optional, default `0644`)

* `vim_sets`: [default: see `defaults/main.yml`]: Set commands

## Dependencies

None

#### Example

```yaml
---
- hosts: all
  roles:
  - vim
```

#### License

MIT

#### Author Information

Mischa ter Smitten

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Oefenweb/ansible-vim/issues)!
