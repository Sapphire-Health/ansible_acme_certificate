ansible-galaxy install -r roles/requirements.yml
ansible-galaxy collection install -r collections/requirements.yml

#run playbook using external vars
ansible-playbook -e @nocsr.yml main.yml

#run playbook using host vars
ansible-playbook -i hosts.yml main.yml