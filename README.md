$ANSIBLE_CONFIG=/opt/ansible-web.cfg ansible-playbook playbook.yml
/etc/ansible/ansible.cfg
/opt/ansible-web.cfg
.ansible.cfg

$ export ANSIBLE_GATHERING=explicit
$ ansible-playbook playbook.yml


$ ansible-config view # Shows the current config file
$ ansible-config list # Lists all configurations
$ ansible-config dump # Shows the current settings
$ export ANSIBLE_GATHERING=explicit
ansible-config dump | grep GATHERING
DEFAULT_GATHERING(env: ANSIBLE_GATHERING) = explicit

/opt/web-playbooks/ansible.cfg --- gathering = explicit


ansible-playbook -i hosts.yml merchantware-dev-api.yml -vv - run playbook
