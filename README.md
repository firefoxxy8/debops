## apparmor

[![Travis CI](http://img.shields.io/travis/ypid/ansible-apparmor.svg?style=flat)](http://travis-ci.org/ypid/ansible-apparmor)
[![Ansible Galaxy](http://img.shields.io/badge/galaxy-ypid.apparmor-660198.svg?style=flat)](https://galaxy.ansible.com/list#/roles/3015)
[![Platforms](http://img.shields.io/badge/platforms-debian-lightgrey.svg?style=flat)](#)


Configure apparmor.

See [Apparmor in the Debian Wiki](https://wiki.debian.org/AppArmor/HowToUse).

By default (e.g. no auditd installed) log messages are logged via syslog to
the kernel facility which usually ends up under /var/log/kern.log.

### Installation

This role requires at least Ansible `v1.3`. To install it, run:

    ansible-galaxy install ypid.apparmor

To install via git, run either:

    git clone https://github.com/ypid/ansible-apparmor ypid.apparmor
    git submodule add https://github.com/ypid/ansible-apparmor roles/ypid.apparmor




### Role variables

List of default variables available in the inventory:

    ---
    
    apparmor_packages:
      - apparmor
      - apparmor-utils
      - apparmor-profiles
      - apparmor-profiles-extra
      - apparmor-notify
    
    apparmor_additional_kernel_parameters: ''
    apparmor_enable: True




### Authors and license

`apparmor` role was written by:

- [Robin Schneider](https://github.com/ypid) | [e-mail](mailto:ypid@riseup.net)

License: [AGPLv3](https://tldrlegal.com/license/gnu-affero-general-public-license-v3-%28agpl-3.0%29)

***

README generated by [Ansigenome](https://github.com/nickjj/ansigenome/).
