This playbook installs Ansible AWX on CentOS7.

## Install Ansible AWX 

Change to root and execute commands below.

```
yum install python-pip git
pip install ansible
git clone https://github.com/ansible-centos7/ansible-awx.git
cd ansible-awx
ansible-galaxy install -r roles/requirements.yml
ansible-playbook -i localhost, -c local install.yml
```
