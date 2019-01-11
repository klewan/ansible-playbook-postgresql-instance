Ansible Playbook: postgresql-instance
=====================================

Create or remove a PostgreSQL instance (cluster)

Supported OS:
-------------
* RedHat
* CentOS
* OracleLinux

Requirements
------------

This playbook requires the postgresql-instance role.

`$ ansible-galaxy install -r roles/requirements.yml`

Examples
--------

    $ ansible-playbook playbook.yml --list-tasks
    $ ansible-playbook playbook.yml --list-tags

Deploy PostgreSQL instance (cluster)

    $ ansible-playbook playbook.yml

Install binaries only

    $ ansible-playbook playbook.yml --tags=postgresql_instance_install_binaries
	
Create or update all config files

    $ ansible-playbook playbook.yml --tags=postgresql_instance_config_files

Update postgresql.auto.conf config file

    $ ansible-playbook playbook.yml --tags=postgresql_instance_postgresql_auto_conf
	
Update pg_hba.conf config file

    $ ansible-playbook playbook.yml --tags=postgresql_instance_hba_conf
	
Update recovery.conf config file

    $ ansible-playbook playbook.yml --tags=postgresql_instance_recovery_conf

Reload Postgres config

    $ ansible-playbook playbook.yml --tags=postgresql_instance_reload_config
		
Create users

    $ ansible-playbook playbook.yml --tags=postgresql_instance_users

Create databases

    $ ansible-playbook playbook.yml --tags=postgresql_instance_databases

	
License
-------

GPLv3 - GNU General Public License v3.0

Author Information
------------------

This playbook was created in 2018 by [Krzysztof Lewandowski](mailto:Krzysztof.Lewandowski@fastmail.fm).


