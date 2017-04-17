Ansible role that deploys a fresh TTRSS server using NGINX and MySQL server.

<<<<<<< HEAD
Can also import existing TTRSS MySQL DB as an option.

FTW!
=======
Example playbook

---

- hosts: ttrss-server
  roles:
    - { role: ansible-ttrss, ttrss_db_password: secret }
>>>>>>> a78947bece6e654ff6b14c80f7ec4fe2bf3723e9
