# ansible-fusuma

[![Build Status](https://travis-ci.org/gsvitins/omz.svg?branch=master)](https://travis-ci.org/gsvitins/ansible-fusuma)
[![Ansible Galaxy](https://img.shields.io/badge/galaxy-gsvitins.ansible--fusuma-blue)](https://galaxy.ansible.com/gsvitins/ansible_fusuma)


# ansible-fusuma
Installs [fusuma multitouch gestures](https://github.com/iberianpig/fusuma) via ansible. Fusuma lets you bind 3 or 4 finger multitouch touchpad systemwide gestures.

Role variables
--------------
```yaml
fusuma_packages:
  - libinput-tools
  - ruby
  - xdotool
fusuma_config_dir: "~/.config/fusuma"
fusuma_config: "config.yml"
fusuma_binary: "/usr/local/bin/fusuma"
fusuma_service_file: "/etc/systemd/system/fusuma.service"

```

Examples
--------
```yaml
- hosts: all
  roles:
    - ansible-fusuma
```
Install via ansible galaxy:
```bash
ansible-galaxy install gsvitins.ansible-fusuma
```
License
-------
MIT License

Dependencies
------------
None
