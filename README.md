# setup git

```
sudo apt install git
git config --global user.email "youremail@gmail.com"
git config --global user.name "yourname"
```

# clone github repository and push a change

```
git clone https://github.com/rbenyounes/ansible
git remote set-url origin git@github.com:rbenyounes/ansible.git
git add README.md
git commit -m "comment"
git push
```

# configure ansible target machines

Make sure the hosts was added to `/etc/ansible/hosts`
```
sudo vim /etc/ansible/hosts
```

```
192.168.0.101 ansible_user=admin
192.168.0.102 ansible_user=admin
```

# run ansible-playbook

```
ansible-playbook cleanup-packages.yml --ask-become-pass

ansible-playbook baseline-setup.yml --ask-become-pass
```
