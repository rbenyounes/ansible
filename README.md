# ansible

git clone https://github.com/rbenyounes/ansible

Make sure the hosts was added to /etc/ansible/hosts
sudo vim /etc/ansible/hosts

ansible-playbook cleanup-packages.yml --ask-become-pass

ansible-playbook baseline-setup.yml --ask-become-pass
