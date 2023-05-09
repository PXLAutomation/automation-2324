test_role
=========

This is a role created for demonstration purposes that configures a basic nginx webserver with a minimal configuration.

Requirements
------------

* Ansible
* Jinja2

Role Variables
--------------

### defaults/main.yml
Default nginx installation variables.
 
* nginx_version: Specific version of nginx to install
* nginx_custom_directory: Custom directory for nginx installation
 
### vars/main.yml
Here we define variables that have high precedence and aren't intended to be changed by the play.
 
* nginx_custom_directory: Custom directory for nginx installation

Dependencies
------------

none

Example Playbook
----------------

   - hosts: all
     become: true
     roles:
       - test_role

License
-------

MIT

Author Information
------------------

Tom Cool
