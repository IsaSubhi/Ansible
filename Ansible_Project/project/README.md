Ansible Main Project
=========

- This Project installs the necessary packages and update the system
- Install webserver Apache/HTTPD
- Copies the project files (HTML) to the hosts
- Prints how many RedHat Debian hosts there are

Requirements
------------

Configuration of the [Ansible Configuration](../ansible.cfg) file and [Hosts](..//hosts) / [Hosts-AWS](../hosts-AWS) file IS REQUIERED

Role Variables
--------------

All Variables can be found in the [VARS](../project/vars/main.yml) file 

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - name: Install Custom Apache Web Server with roles
      hosts: all
      become: yes  # Run tasks with sudo privileges
      roles:
        - { role: project }
