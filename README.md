Composer
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
    composer_path: /usr/local/bin/composer

    # Path to Composer vendor binaries.
    composer_bin_dir: /home/vagrant/.composer/vendor/bin

Dependencies
------------

 - None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: webservers
      roles:
         - { role: AlexanderAllen.Composer }

Inside `vars/main.yml`:

    ---
    composer_path: /usr/local/bin/composer
    composer_bin_dir: /home/myusername/.composer/vendor/bin

License
-------

GPLv2

Author Information
------------------

https://github.com/AlexanderAllen
