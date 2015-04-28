# Openresty

Configures and installs openresty

## Requirements

- Ansible 1.2+
- Ubuntu 14.04+


## Variables

### Openresty

| Name 						| Default 								| Description 							|
|---------------------------|-------------------------------------------------------------------------------|
| openresty_version			| 1.7.7.2 								| Openresty Version 					|
| with_luajit				| true									| Configure parameter					|
| with_dav					| true									| Configure parameter					|
| with_flv					| true									| Configure parameter					|
| with_geoip				| true									| Configure parameter					|
| with_gzip_static			| true									| Configure parameter					|
| with_image_filter			| true									| Configure parameter					|
| with_realip				| true									| Configure parameter					|
| with_stub_status			| true									| Configure parameter					|
| with_ssl 					| true									| Configure parameter					|
| with_sub 					| true									| Configure parameter					|
| with_xslt					| true									| Configure parameter					|
| with_ipv6					| true									| Configure parameter					|
| with_sha1					| "/usr/include/openssl"				| Configure parameter					|
| with_md5					| "/usr/include/openssl"				| Configure parameter					|
| with_mail 				| true									| Configure parameter					|
| with_mail_ssl				| true									| Configure parameter					|
| with_stub_status			| true									| Configure parameter					|
| with_secure_link			| true									| Configure parameter					|
| with_sub 					| true									| Configure parameter					|

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