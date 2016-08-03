Role Name
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

The following default variables are set which can be overridden

console_phar_url: https://drupalconsole.com/installer
phar_destination: ~/drupal.phar
drupal_cmd_destination: /usr/local/bin/drupal

Dependencies
------------

This role requires PHP to be installed on the target. I recommend geerlingguy.php

Example Playbook
----------------

Add the following into your requirements.yml

- src: https://github.com/mikedarke/ansible-d8console
  version: master
  name: mdarke.d8console

Add the role to your playbook:

    - hosts: servers
      roles:
         - { role: mdarke.d8console }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
