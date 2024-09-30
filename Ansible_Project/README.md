# Ansible Project:
## Overview:
[Main Project](./project):
- This Project install the necessary packages
- Update the system
- Install webserver Apache/HTTPD
- Copies the project files (HTML) to the hosts
- Prints how many RedHat Debian hosts there are
<br>

[Training Project](./training_project):
- Copies 1.txt file to the host
- Prints a message
- Prints OS_FAMILY of host
- Creates and prints a var
- Saves IP address of host to log.txt
- Reboots host and save the time of the reboot to log.txt

## Usage:

To run the Projects it is necessary to configure the [Ansible Configuration](./ansible.cfg) file AND [Hosts](./hosts) / [Hosts-AWS](./hosts-AWS) file.<br>
<br>
The projects can be executed by running:<br> 
[Project](./run_project.yaml) run file: <br> 

    - name: Install Custom Apache Web Server with roles
      hosts: all
      become: yes  # Run tasks with sudo privileges
      roles:
        - { role: project }
  
[Training Project](./run_training_project.yaml) run file:

    - name: Run training_project
      hosts: all
      become: yes
      roles:
        - { role: training_project }
