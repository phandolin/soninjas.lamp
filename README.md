Ansible Role: LAMP
=========

Simple installation of a LAMP stack on RHEL/CentOS

Requirements

Sample centos playbook file:
--------------

    hosts: centos-webserver
    remote_user: ansible
    become: true

    vars_files:
      - "../roles/soninjas.lamp/vars/main.yml"

    roles:
         - role: soninjas.lamp
           tags: lamp


Role Variables
--------------

You can change the document root of Apache in `vars/main.yml` . You are free to change any part of the role and adapt it to your needs

Author Information
------------------
Southern Oregon Net Ninjas contact: phil@southernoregonnetninjas.com
