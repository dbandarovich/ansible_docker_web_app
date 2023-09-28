Role Name
=========

This is a role that configures a basic nginx webserver with 2 virtual hosts.

Requirements
------------

Any prerequisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

* Ansible
* Jinja2

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Default nginx installation variables.

### defaults/main.yml
* destination_folder: remote absolute path where the file should be copied to.


Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    ---
    - hosts: all
      become: yes

      roles:
        - { role: deploy_nginx_web, when ansible_system == 'Linux' }

License
-------

NGINX

Author Information
------------------

Dmitry Bandarovich
