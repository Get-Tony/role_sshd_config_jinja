sshd_config
=========

Deploy an OS independent sshd_config file.

Requirements
------------

None.

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

    sshd_pkg_state
    sshd_port
    sshd_permit_root_login
    sshd_host_keys
    sshd_listen_addresses
    sshd_password_authentication
    sshd_print_motd

Dependencies
------------

None.

Example Playbook
----------------

    - name: Assure sshd_config
      hosts: managed
      roles:
        - role: sshd_config
          vars:
            sshd_port: 22
            sshd_permit_root_login: yes

License
-------

This project is licensed under the MIT License.

Author Information
------------------

This role was created in 2022 by Anthony Pagan.
