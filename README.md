# test
---
# WEB SERVER

- hosts: serverweb
  become: true

  tasks:
  - name: install apache and php last version
    apt:
      name:
        - apache2
        - php
        - php-mysql
      state: present
      ...
