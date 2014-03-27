ansible-selenium-role
=====================

role to install and configure the selenium server
=======
Role Name
========

This role installs the selenium server

Requirements
------------

This role requires the java, currently to supply this it depends on the oracle_java7 role

Role Variables
--------------

# info for downloading seleinum verion
download_url: http://selenium.googlecode.com/files/{{jar_file}}
jar_file: selenium-server-standalone-{{server_version}}.jar
server_version: 2.39.0

# roles can be: standalone, hub or node
sel_role: standalone

##### optional vars #####
# uri for slaves to find hub server
hub: ''
# jvm settings
java_opts: ''
# extra arguments to selenium jar
extra_args: ''
# specific port for selemium server (uses selenium role default otherwise)
port: ''



Dependencies
------------

It depends on the oracle_java7 role

License
-------

GPLv2

Author Information
------------------

briancoca+selenium@gmail.com
