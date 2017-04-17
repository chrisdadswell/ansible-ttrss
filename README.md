Ansible role that deploys a fresh TTRSS server using NGINX and MySQL server.

Example playbook

<code>

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
  
</code>

