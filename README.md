# `dotfiles-role-sublime`
# `dotfiles-role-sublime`

[![Build Status](https://travis-ci.org/thecjharries/dotfiles-role-sublime.svg?branch=master)](https://travis-ci.org/thecjharries/dotfiles-role-sublime)
[![Build Status](https://travis-ci.org/thecjharries/dotfiles-role-sublime.svg?branch=master)](https://travis-ci.org/thecjharries/dotfiles-role-sublime)

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
- src: git+https://github.com/thecjharries/dotfiles-role-common-software.git
- src: git+https://github.com/thecjharries/dotfiles-role-common-software.git
- src: git+https://github.com/thecjharries/dotfiles-role-package-installer.git
- src: git+https://github.com/thecjharries/dotfiles-role-package-installer.git
```

## Example Playbook

```yml
---
- hosts: all

  roles:
    - role: dotfiles-role-sublime
    - role: dotfiles-role-sublime
```

## License

ISC
