Ansible Telegraf (Influxdata) role
=========

Simple role that installs Telegraf on your server and copies config.

Requirements
------------

Ansible 2.0 and Ubuntu on the server.

Role Variables
--------------

Telegraf package URL:

`telegraf_deb_url: https://dl.influxdata.com/telegraf/releases/telegraf_1.3.3-1_amd64.deb`

This role has no configuration template. You need create custom configuration file `telegraf.conf`, after that set variable `telegraf_config_file_path`.
That file will copy to system telegraf config path `/ect/telegraf/telegraf.conf`.

Dependencies
------------
No

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: salex-ansible.telegraf }

License
-------

BSD

