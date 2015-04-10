# Ansible Role For Ruby

[![Build Status](https://img.shields.io/circleci/project/crushlovely/ansible-ruby.svg?style=flat)](https://github.com/crushlovely/ansible-ruby)
[![Current Version](http://img.shields.io/github/release/crushlovely/ansible-ruby.svg?style=flat)](https://galaxy.ansible.com/list#/roles/1180)

This Ansible role installs `ruby` and `bundler`.

We use this to install Ruby when required.

## Installation

``` bash
$ ansible-galaxy install crushlovely.ruby,v2.0.0
```

## Variables

``` yaml
ruby
  mversion: 2.0
  fversion: 2.0.0-p576
  cversion: 2.0.0p576
app:
  user: ubuntu
  group: ubuntu
```

## Usage

Once this role is installed on your system, include it in the roles list of your playbook.

``` yaml
---
- hosts: localhost
  roles:
    - crushlovely.ruby
```

## Dependencies

None

## License

MIT