## vim [![Build Status](https://travis-ci.org/Oefenweb/ansible-vim.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-vim)

Set up vim in Debian-like systems.

#### Requirements

None

#### Variables

* `vim_vimrc_destinations`: [default: `[/etc/skel, {{ ansible_env.HOME }}]`]: Destinations to copy the vimrc file to
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
