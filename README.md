[![Build Status](https://travis-ci.org/tumf/ansible-role-docker-compose.svg?branch=master)](https://travis-ci.org/tumf/ansible-role-docker-compose)
[![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-docker--compose-blue.svg)](https://galaxy.ansible.com/tumf/docker-compose/)

ansible-role-docker-compose
===========================

Install Docker Compose Ansible Role

Requirements
------------


Role Variables
--------------

|name|type|default|description
|----|----|-------|-----------
|ansible_unit_test|boolean|false|unit testing?
|prefix_dir|string|""|prefix directory for testing
|docker_compose_arch|string|"Linux-x86_64"|
|docker_compose_version|string|"latest"|
|docker_compose_release_url|string|"https://github.com/docker/compose/releases/download"|
|docker_compose_bin|string|"/usr/local/bin"|install path


Example Playbook
----------------

    - Host: servers
      connection: local
      roles:
        - role: tumf.docker-compose
        docker_compose_version: 1.5.2

License
-------

MIT

Author Information
------------------

> @tumf
