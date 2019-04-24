# Steps to Using Ansible

1. Check the playbook has a requirement or not
   
   if the playbook file name is `playbook.yml`
   then playbook requirement filename is `playbook-requirements.yml`

2. Skip this step if the playbook does not have requirement
   
   run `ansible-galaxy install -r playbooks/playbook-requirements.yml`

3. run `ansible-playbook playbooks/playbook.yml -i hosts/development`
   
   current command for development environment only, if in production change the environment to `hosts/production`

4. Voila done :)