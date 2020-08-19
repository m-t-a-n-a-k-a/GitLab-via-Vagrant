# GitLab-via-Vagrant
Vagrantfile and Ansible playbook for provisioning testing GitLab environment

## Overview
This repo provides Vagrantfile and Ansible playbook for provisioning testing GitLab with gitlab-runner environment.

## Getting Started
### Prerequisites
- Vagrant
- VirtualBox
- git

### Setup
Clone this repo and change the current directory.

```
$ cd ~/
$ git clone https://github.com/m-t-a-n-a-k-a/GitLab-via-Vagrant.git
$ cd GitLab-via-Vagrant/
```

Check the VM to be created.
```
$ vagrant status
Current machine states:

gitlab01                  not created (virtualbox)
```

Create and provision the VM.
```
$ vagrant up --provision
```

Access the Web UI(192.168.11.11 via default settings in Vagrantfile) and continue setup.
