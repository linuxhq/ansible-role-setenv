# ansible-role-setenv

[![Build Status](https://travis-ci.org/linuxhq/ansible-role-setenv.svg?branch=master)](https://travis-ci.org/linuxhq/ansible-role-setenv)
[![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-setenv-blue.svg?style=flat)](https://galaxy.ansible.com/linuxhq/setenv)
[![License](https://img.shields.io/badge/license-GPLv3-brightgreen.svg?style=flat)](COPYING)

RHEL/CentOS - Set local environment variables

## Requirements

This role requires that your inventory hostname be in the following format:

    class.product.env.tld

Examples:

    tkimball83.plex.linuxhq.org
    glkimball5456.plex.linuxhq.org
    cloudpro.cac.linuxhq.org
    kahu.lc.linuxhq.org

## Role Variables

None

## Dependencies

None

## Example Playbook

    - hosts: servers
      roles:
        - role: linuxhq.setenv

Assuming your inventory hostname is tkimball83.plex.linuxhq.org, this role will produce the following variables.

    local_class: tkimball83
    local_product: plex
    local_env: linuxhq
    local_tld: org
    local_fqdn: tkimball83.plex.linuxhq.org
    local_domain: linuxhq.org
    local_search: plex.linuxhq.org

## License

Copyright (C) 2018 Taylor Kimball <tkimball@linuxhq.org>

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <http://www.gnu.org/licenses/>.
