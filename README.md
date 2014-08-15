# Ansible Role For Ruby

[![Build Status](http://img.shields.io/travis/crushlovely/ansible-ruby.svg?style=flat)](https://travis-ci.org/crushlovely/ansible-deploy-user)
[![Current Version](http://img.shields.io/github/release/crushlovely/ansible-ruby.svg?style=flat)](https://galaxy.ansible.com/list#/roles/1180)

This Ansible role that installs `ruby` and `bundler`.

We use this to install Ruby when required.

## Installation

``` bash
$ ansible-galaxy install crushlovely.ruby
```

## Variables

``` yaml
ruby_mversion: 2.0
ruby_fversion: 2.0.0-p247
ruby_cversion: 2.0.0p247
```

## Usage

Once this role is installed on your system, include it in the roles list of your playbook.

``` yaml
---
- hosts: localhost
  roles:
    - { role: crushlovely.ruby, ruby_mversion: 2.0, ruby_fversion: 2.0.0-p247, ruby_cversion: 2.0.0p247 }
```

## Dependencies

This role requires there to be a `deploy` user with sudo capabilities.  [Click here to view our users role](https://galaxy.ansible.com/list#/roles/1337)


## License

MIT