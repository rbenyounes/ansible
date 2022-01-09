# github

clone the Git repository
```
git clone https://github.com/rbenyounes/ansible
git remote set-url origin git@github.com:rbenyounes/ansible.git
git add README.md
git commit -m "comment"
git push
```

# ansible

Make sure the hosts was added to /etc/ansible/hosts
sudo vim /etc/ansible/hosts

ansible-playbook cleanup-packages.yml --ask-become-pass

ansible-playbook baseline-setup.yml --ask-become-pass
