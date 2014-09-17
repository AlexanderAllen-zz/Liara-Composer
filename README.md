Liara/Composer
=============

Ansible role for installing Composer.

Requirements
------------

- PHP

Role Variables
--------------

This role installs composer to `composer_path` and makes any binaries downloaded by Composer
to `composer_bin_dir` available to the environment through `/etc/environment`.

Variables specified in `vars/main.yml`:

    # Path to the Composer executable.
    liara_composer_path: /usr/local/bin/composer

    # Path to Composer vendor binaries.
    liara_composer_bin_dir: /home/vagrant/.composer/vendor/bin

Dependencies
------------

 - None.

Example Playbook
----------------

    - hosts: webservers
      roles:
         - { role: AlexanderAllen.Liara-Composer }

Inside `vars/main.yml`:

    ---
    liara_composer_path: /usr/local/bin/composer
    liara_composer_bin_dir: /home/myusername/.composer/vendor/bin

License
-------

GPLv2

Author Information
------------------

https://github.com/AlexanderAllen
