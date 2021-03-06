# `dotfiles-role-package-installer`

[![Build Status](https://travis-ci.org/thecjharries/dotfiles-role-package-installer.svg?branch=master)](https://travis-ci.org/thecjharries/dotfiles-role-package-installer)
[![GitHub tag](https://img.shields.io/github/tag/thecjharries/dotfiles-role-package-installer.svg)](https://github.com/thecjharries/dotfiles-role-package-installer)

An Ansible role that installs packages in my dotfiles on Fedora 27,

## Requirements

Fedora 27 is recommended.

## Role Variables

Defaults are below.

    desired_state: "latest"
    packages_to_install:

`packages_to_install` should be a list of packages to install.

## Dependencies

None

## Example Playbook

    - hosts: all

    roles:
      - role: dotfiles-role-package-installer
        packages_to_install:
          - xclock

## License

ISC
