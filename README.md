# ansible-meehan

My Ansible scripts for setting up my Raspberry Pis.  Based on: [raspberry-ansible](https://github.com/rhietala/raspberry-ansible).

Mostly edited so I could reuse an existing UFW role, and refactored so that the bulk of the Debian bootstrap is loaded as an external role.

To run:

```
ansible-galaxy install -r requirements.yml
ansible-playbook -i hosts bootstrap.yml 
```

This command should work before hand: `ansible -i hosts all -m ping`

