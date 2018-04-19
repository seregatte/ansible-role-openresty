# OpenResty
Configures and installs [OpenResty NGINX](https://openresty.org/en/)

[![Build Status](https://travis-ci.org/HauptJ/ansible-role-openresty.svg?branch=master)](https://travis-ci.org/HauptJ/ansible-role-openresty)

## Requirements
- Ansible 2.3+
- CentOS 7.4+
- Ubuntu 16.04+ [**SOURCE INSTALL ONLY**]

## Installation
1. Fork this repository
2. git submodule add <git host> roles/ansible-role-openresty
    - [submodule reference](https://chrisjean.com/git-submodules-adding-using-removing-and-updating/)

**Ansible Galaxy:** [HauptJ.openresty](https://galaxy.ansible.com/HauptJ/openresty/)

## Variables

### Openresty

| Name 						            | Default 							                    | Description 										   |
|-----------------------------|-------------------------------------------|------------------------------------|
| resty_install_from_source   | true                                      | Install from source [**true**] or from repository [**false**]|
| resty_compile_threads       | 2                                         | Number of threads to use to configure and compile |
| resty_default_server        | true                                      | Setup default (welcome) webserver and webpage     |
| resty_default_web_dir       | /usr/local/openresty/nginx/html/default   | default web directory              |
| resty_sites_dir             | /usr/local/openresty/nginx/sites          | sites / vhost directory            |
| resty_web_user              | nginx                                     | OpenResty web service user and group |
| resty_conf_dir              | /usr/local/openresty/nginx/conf           | Configuration file directory       |
| resty_log_dir               | /var/log/openresty                        | Log file directory                 |
| openresty_version	          | 1.11.2.5 				                          | OpenResty Version 								 |
| with_luajit				          | true									                    | Compile with luajit support 			 |          
| with_dav					          | true									                    | Compile with dav support 					 |          
| with_flv					          | true									                    | Compile with flv support 					 |           
| with_geoip				          | true									                    | Compile with geoip support 				 |          
| with_gzip_stati		          | true							                        | Compile with gzip_static support 	 |          
| with_image_filter	          | true						    	                    | Compile with image_filter support  |          
| with_realip				          | true									                    | Compile with realip support 			 |          
| with_stub_status	          | true						     	                    | Compile with stub_status support 	 |          
| with_ssl 					          | true									                    | Compile with ssl support 					 |          
| with_sub 					          | true									                    | Compile with sub support 					 |          
| with_xslt					          | true									                    | Compile with xslt support 				 |          
| with_ipv6					          | true									                    | Compile with IPv6 support    			 |          
| with_sha1					          | "/usr/include/openssl"				            | Compile with sha1 support [**DEPRECIATED**] |          
| with_md5					          | "/usr/include/openssl"				            | Compile with md5 support [**DEPRECIATED**] 	|         
| with_mail 				          | true								 	                    | Compile with mail support 				 |          
| with_mail_ssl			          | true						   	                      | Compile with mail_ssl support 		 |          
| with_secure_link	          | true							                        | Compile with secure_link support 	 |          
| with_pcre_jit 		          | true							   	                    | Compile with pcre jit support 	 	 |          
| with_debug 				          | true									                    | Compile with debug module 				 |          
| with_auth_request           | true						    	                    | Compile with auth_request module 	 |          
| with_addition 		          | true									                    | Compile with addition_module  		 |          
| with_gunzip 			          | true									                    | Compile with gunzip module			 	 |          
| with_postgres 		          | true									                    | Compile with PostgreSQL support		 |
| with_http2                  | true                                      | Compile with http2 support         |
| with_file_aio               | true                                      | Compile with file AIO              |


Dependencies
------------

None


Example Playbook
----------------

Including an example of how to use your role:

    - hosts: webservers
      roles:
         - ansible-role-openresty

License
-------

MIT

Author Information
------------------

1. [João Paulo Seregatte](https://github.com/seregatte) <seregatte@gmail.com>
  - Forked from: [ansible-role-openresty](https://github.com/seregatte/ansible-role-openresty)
2. [Joshua Haupt](https://hauptj.com/) <josh@hauptj.com>
