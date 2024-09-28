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

How to use the role:<br>
By running [Project Run](../run_project.yaml) file 

    - name: Install Custom Apache Web Server with roles
      hosts: all
      become: yes  # Run tasks with sudo privileges
      roles:
        - { role: project }
