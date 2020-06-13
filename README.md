# Ansible

once after ansible is installed on server(controller), make a passwordless conection to remote servers(nodes)

add below in /etc/ansible/hosts on server(controller)

[remote:vars]
ansible_host=<remote ip>
ansible_ssh_private_key_file=~/.ssh/id_rsa
ansible_user=<user>
  
  
execution steps:
to install docker and docker-compose
cmd: ansible-playbook install-docker_dockercompose-playbook.yml

to uninstall docker and docker-compose
cmd: ansible-playbook uninstall-docker_dockercompose-playbook.yml
