ansible-selenium-role
=====================

This role installs the selenium server

Requirements
------------

This role requires the java, currently to supply this it depends on the oracle_java7 role

Role Variables
--------------

Info for downloading seleinum version

    download_url: http://selenium.googlecode.com/files/{{jar_file}}
    jar_file: selenium-server-standalone-{{server_version}}.jar
    server_version: 2.39.0

Roles can be: standalone, hub or node

    sel_role: standalone

URI for slaves to find hub server

    hub: ''

Jvm settings

    java_opts: ''

Extra arguments to selenium jar

    extra_args: ''

Specific port for selemium server (uses selenium role default otherwise)

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
