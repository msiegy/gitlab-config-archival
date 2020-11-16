# gitlab-config-archival

Ansible gitlab-config-archival
- Pull configs with Ansible
- Check for changes
- Merge changes and Commit

How To Use:

1) Setup local ansible server with gitlab SSH keys for your repo and configure global git username.
   - ssh-keygen -t rsa
   - copy private key to gitlab SSH Keys
   - git config --glboal user.name "user"
   - git config --global user.email "email@email.com"
2) Create Repo in gitlab
2) git clone the gitlab repo on your local ansible server
3) Configure host file
4) Run: ansible-playbook conf2gitlab.yml -i hosts.ini
