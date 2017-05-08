# OSX Development Environment
Prepare the OSX environment for development with Ansible

## Installation

### Step 1: Install Ansible

 - Install [Xcode](https://developer.apple.com/xcode/)
 - Install pip
```Shell
$ sudo easy_install pip
```
 - Install Ansible
```Shell
$ sudo pip install ansible --quiet
```
If you have troubles installing Ansible on MacOS Sierra, try:

```Shell
$ sudo pip install git+http://github.com/ansible/ansible.git@devel
```

### Step 2: Download the project
```Shell
$ git clone git@github.com:linkita/osx-development-environment.git
```

### Step 3: Execute the playbook with all roles
```Shell
$ ansible-playbook -K playbook.yml
```
You can choose which applications install by editing playbook.yml

By default all roles are includes in playbook.yml, so you can delete or comment (with #) those that you don´t want.

