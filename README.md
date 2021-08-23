# Ansible Role: ansible-apps_prometheus_msteams

## Description

[![Build Status](https://travis-ci.com/lotusnoir/ansible-apps_prometheus_msteams.svg?branch=master?style=flat)](https://travis-ci.com/lotusnoir/ansible-apps_prometheus_msteams)
[![License](https://img.shields.io/badge/license-Apache--2.0-brightgreen?style=flat)](https://opensource.org/licenses/Apache-2.0)
[![Ansible Role](https://img.shields.io/badge/galaxy-apps_prometheus_msteams-purple?style=flat)](https://galaxy.ansible.com/lotusnoir/apps_prometheus_msteams)
![GitHub repo size](https://img.shields.io/github/repo-size/lotusnoir/ansible-apps_prometheus_msteams?color=orange&style=flat)
![Ansible Quality Score](https://img.shields.io/ansible/quality/52260)
[![downloads](https://img.shields.io/ansible/role/d/52260)](https://galaxy.ansible.com/lotusnoir/apps_prometheus_msteams)
[![Version](https://img.shields.io/github/release/lotusnoir/ansible-apps_prometheus_msteams.svg)](https://github.com/lotusnoir/ansible-apps_prometheus_msteams/releases/) 
[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=lotusnoir_ansible-apps_prometheus_msteams&metric=alert_status)](https://sonarcloud.io/dashboard?id=lotusnoir_ansible-apps_prometheus_msteams)
[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=lotusnoir_ansible-apps_prometheus_msteams&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=lotusnoir_ansible-apps_prometheus_msteams)
[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=lotusnoir_ansible-apps_prometheus_msteams&metric=reliability_rating)](https://sonarcloud.io/dashboard?id=lotusnoir_ansible-apps_prometheus_msteams)
[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=lotusnoir_ansible-apps_prometheus_msteams&metric=security_rating)](https://sonarcloud.io/dashboard?id=lotusnoir_ansible-apps_prometheus_msteams)


Deploy [prometheus_msteams](https://github.com/momorientes/prometheus_msteams) to expose patroni metrics to prometheus.

## Role variables

| Name                     | Default Value                | Description                           |
| ------------------------ | ---------------------------- | --------------------------------------|
| `prometheus_msteams_port` | 9120                         | port to expose prometheus metrics     |
| `patroni_web_url`       | https://patroni.example.net | web url of the patroni application   |

## Examples

	---
	- hosts: apps_prometheus_msteams
	  become: yes
	  become_method: sudo
	  gather_facts: yes
	  roles:
	    - role: ansible-apps_prometheus_msteams
	  environment: 
	    http_proxy: "{{ http_proxy }}"
	    https_proxy: "{{ https_proxy }}"
	    no_proxy: "{{ no_proxy }}


## Grafana Dashboard

You can find a grafana dashboard [here](https://grafana.com/grafana/dashboards/13556)


## License

This project is licensed under Apache License. See [LICENSE](/LICENSE) for more details.
