## Ansible Role for installing and configuring auditd and rsyslog on Oracle Linux 7 and 8

---

This role is designed specifically to provision OL7 and 8 servers with auditd service and configure its comonenets and rsyslog for logs shipping.
OL distrib version is determined based on facts: "ansible_distribution" and "ansible_distribution_major_version" 

---

### Example of Role file:

<pre>
  ---
- name: Install and configure audit
  hosts: allhosts
  remote_user: root
  roles:
    - audit_set

</pre>
---

