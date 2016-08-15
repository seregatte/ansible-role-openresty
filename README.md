# Openresty

Configures and installs openresty

## Requirements

- Ansible 1.2+
- Ubuntu 14.04+

## Installation

```shell
$ ansible-galaxy install seregatte.openresty
```

## Variables

### Openresty

| Name 						| Default 								| Description 										|
|---------------------------|---------------------------------------|---------------------------------------------------|
| openresty_version			| 1.9.15.1 								| Openresty Version 								|
| with_luajit				| true									| Compile with luajit support 						|          
| with_dav					| true									| Compile with dav support 							|          
| with_flv					| true									| Compile with flv support 							|          
| with_geoip				| true									| Compile with geoip support 						|          
| with_gzip_static			| true									| Compile with gzip_static support 					|          
| with_image_filter			| true									| Compile with image_filter support 				|          
| with_realip				| true									| Compile with realip support 						|          
| with_stub_status			| true									| Compile with stub_status support 					|          
| with_ssl 					| true									| Compile with ssl support 							|          
| with_sub 					| true									| Compile with sub support 							|          
| with_xslt					| true									| Compile with xslt support 						|          
| with_ipv6					| true									| Compile with ipv support 							|          
| with_sha1					| "/usr/include/openssl"				| Compile with sha support 							|          
| with_md5					| "/usr/include/openssl"				| Compile with md support 							|          
| with_mail 				| true									| Compile with mail support 						|          
| with_mail_ssl				| true									| Compile with mail_ssl support 					|          
| with_secure_link			| true									| Compile with secure_link support 					|          
| with_pcre_jit 			| true									| Compile with pcre jit support 					|          
| with_debug 				| true									| Compile with debug module 						|          
| with_auth_request 		| true									| Compile with auth_request module					|          
| with_addition 			| true									| Compile with addition_module  					|          
| with_gunzip 				| true									| Compile with gunzip module						|          
| with_postgres 			| true									| Compile with PostgreSQL support					|          

Dependencies
------------

None


Example Playbook
----------------

Including an example of how to use your role:

    - hosts: webservers
      roles:
         - seregatte.openresty

License
-------

MIT

Author Information
------------------

João Paulo Seregatte <seregatte@gmail.com>