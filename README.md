ansible-selenium-extra-role
=====================

This role installs the selenium server using selenium grid extras project [Selenium-Grid-Extras](https://github.com/groupon/Selenium-Grid-Extras)

Requirements
------------

This role requires the java, currently to supply this it depends on the oracle_java7 role

Role Variables
--------------

Info for downloading seleinum version

    server_version_major: 2.52
    server_version: "{{server_version_major}}.0"
    grid_extras_version: 1.11.8
    chrome_driver_version: 2.21
    ie_driver_version: 2.53.1
    max_sessions: 5
    sel_role: hub
    run_xvfb: 1

Roles can be: hub or node

    sel_role: node

URI for slaves to find hub server

    hub_host: ''

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

Credits
------------------

Based on [github/ansible-selenium-role](https://github.com/bcoca/ansible-selenium-role)

