--------
Vagrant will automatically generate a rsa key when vagrant up (see vagrant ssh-config)

For Ansible to provision the vm with config, we need to allow ssh from Ansible.

1/ vagrant ssh into said guest machine
2/ setup passwordAuth = yes in /etc/ssh/sshd-config?
3/ change ansible inventory file to supply ansible_ssh_user and ansible_ssh_pass
