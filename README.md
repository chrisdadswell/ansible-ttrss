Ansible role that deploys a fresh TTRSS server using NGINX and MySQL server.

Example playbook

---

- hosts: ttrss-server
  roles:
    - { role: ansible-ttrss, ttrss_db_password: secret }
