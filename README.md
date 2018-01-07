# `dotfiles-sublime-role`

[![Build Status](https://travis-ci.org/thecjharries/dotfiles-sublime-role.svg?branch=master)](https://travis-ci.org/thecjharries/dotfiles-sublime-role)

## Requirements

Fedora 27 is recommended.

## Role Variables

Defaults are below.

```yml
---
owning_user: "{{ ansible_user }}"
owning_group: "{{ ansible_user }}"
root_dir: "/home/{{ ansible_user }}"
config_dir: "{{ root_dir }}/.config"
```

## Dependencies

```yml
---
- src: git+https://github.com/thecjharries/dotfiles-common-software-role.git
- src: git+https://github.com/thecjharries/dotfiles-package-installer-role.git
```

## Example Playbook

```yml
---
- hosts: all

  roles:
    - role: dotfiles-sublime-role
```

## License

ISC
