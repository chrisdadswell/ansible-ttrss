Ansible role that deploys a fresh TTRSS server using Apache and MySQL server.

This playbook has been created to run via Jenkins and resolve dependencies from a local OSS Artifactory repo.

Example playbook

```

---

- hosts: ttrss-server
  roles:
    - { role: ansible-ttrss, 
    ttrss_user_password: "{{ ttrss_user_passwd }}",
    ttrss_db_password: "{{ ttrss_db_passwd }}",
    ttrss_arty_passwd: "{{ ttrss_arty_passwd }}",
    ttrss_self_url: "{{ ttrss_self_url }}"
    }
    
  become_user: root  
  become_method: sudo
  
```

