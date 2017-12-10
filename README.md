# ansible-role-setenv

[![Build Status](https://travis-ci.org/linuxhq/ansible-role-setenv.svg?branch=master)](https://travis-ci.org/linuxhq/ansible-role-setenv)

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

There are no default variables for this role.

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

GPLv3

## Author Information

This role was created by [Taylor Kimball](http://www.linuxhq.org).
