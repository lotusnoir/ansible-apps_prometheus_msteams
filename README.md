# ansible-apps_prometheus_msteams

[![Galaxy Role](https://img.shields.io/badge/galaxy-apps_prometheus_msteams-purple?style=flat)](https://galaxy.ansible.com/lotusnoir/apps_prometheus_msteams)
[![Version](https://img.shields.io/github/release/lotusnoir/ansible-apps_prometheus_msteams.svg)](https://github.com/lotusnoir/ansible-apps_prometheus_msteams/releases/latest)
[![GitHub repo size](https://img.shields.io/github/repo-size/lotusnoir/ansible-apps_prometheus_msteams?color=orange&style=flat)](https://galaxy.ansible.com/lotusnoir/apps_prometheus_msteams)
[![downloads](https://img.shields.io/ansible/role/d/56098)](https://galaxy.ansible.com/lotusnoir/apps_prometheus_msteams)
[![Ansible Quality Score](https://img.shields.io/ansible/quality/56098)](https://galaxy.ansible.com/lotusnoir/apps_prometheus_msteams)
[![License](https://img.shields.io/badge/license-Apache--2.0-brightgreen?style=flat)](https://opensource.org/licenses/Apache-2.0)

## Description

Deploy [prometheus_msteams](https://github.com/momorientes/prometheus_msteams) to send alertmanager alerts to msteams.
## Requirements

none

## Role variables

See [variables](/defaults/main.yml) for more details.

## Examples

        ---
        - hosts: apps_prometheus_msteams
          become: true
          become_method: sudo
          gather_facts: true
          roles:
            - role: ansible-apps_prometheus_msteams


## License

This project is licensed under Apache License. See [LICENSE](/LICENSE) for more details.

## Author Information

- [Philippe LEAL](https://github.com/lotusnoir)
