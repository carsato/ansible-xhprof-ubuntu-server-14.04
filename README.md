ansible-xhprof-ubuntu-server-14.04
===================

Based on https://github.com/qandidate-labs/ansible-lamp-server

Updated for ubuntu server 14.04

#set up your hosts
sudo echo "10.0.0.10 xhgui.local" >> /etc/hosts

#start machine
vagrant up

#install xhprof on vagrant machine
ansible-playbook -i hosts profiling.yml -v
