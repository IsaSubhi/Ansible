Ansible Training Project
=========

- Copies 1.txt file to the host
- Prints a message
- Prints OS_FAMILY of host
- Creates and prints a var
- Saves IP address of host to log.txt
- Reboots host and save the time of the reboot to log.txt

Requirements
------------

Configuration of the [Ansible Configuration](../ansible.cfg) file and [Hosts](..//hosts) / [Hosts-AWS](../hosts-AWS) file IS REQUIERED

Role Variables
--------------

All Variables can be found in the [VARS](../project/vars/main.yml) file

Example Playbook
----------------

How to use the role:<br>
By running [Training Project run](../run_training_project.yaml)  file:

    - name: Run training_project
      hosts: all
      become: yes
      roles:
        - { role: training_project }
