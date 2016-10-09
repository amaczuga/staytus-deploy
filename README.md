# staytus-deploy
Ansible playbook for staytus deployment

A MySQL DBMS needs to be prepared upfront,
then configured in `group_vars/all`.

The inventory file should be filled with
real host names.

```cp inventory/staytus.example inventory/staytus
vim inventory/staytus```

The install command can look like:

```ANSIBLE_HOST_KEY_CHECKING=False ansible-playbook -i inventory/staytus site.yml```

This version has been tested on RHEL 6.5
