wireshark
=========

[![Build Status](https://travis-ci.org/ymajik/ansible-role-wireshark.svg?branch=master)](https://travis-ci.org/ymajik/ansible-role-wireshark)
[![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-wireshark-blue.svg?style=flat)](https://galaxy.ansible.com/ymajik/wireshark)

Ansible role to install wireshark on Debian based systems

Requirements
------------

None

Role Variables
--------------

Set wireshark_gui to true if you want to enable the graphical user interface

```yaml
wireshark_user: "{{ lookup('env','USER') }}"
wireshark_gui: false
wireshark_cli: true
wireshark_gui_package: wireshark
wireshark_cli_package: tshark
```

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: ymajik.wireshark }

License
-------

BSD

Author Information
------------------

ymajik
