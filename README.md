# Openresty

Configures and installs openresty

## Requirements

- Ansible 1.2+
- Ubuntu 14.04+


## Variables

### Openresty

| Name                      | Default  | Description                                                       |
|---------------------------|----------|-------------------------------------------------------------------|
| openresty_version         | 1.7.7.2  | Openresty openresty_version                                       |


Dependencies
------------

None


Example Playbook
----------------

Including an example of how to use your role:

    - hosts: servers
      vars:
         - openresty_version: 1.7.7.2 # Optional because we already have a default value
      roles:
         - ansible-role-openresty

License
-------

MIT

Author Information
------------------

João Paulo Seregatte <seregatte@gmail.com>

TODO
------------

- Put the openresty configure options in ansible vars
- Submit to galaxy.ansible.com