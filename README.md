# ✨ Ansible Magic
## 🔧 Pre (Make your machine Ansible ready)
### [Read this article](https://www.isitix.com/en/blog/technical/how-to-make-a-debian-linux-machine-ansible-readiy) OR
###  🏃‍ Tl;DR 

1. install ssh-server:
```bash
sudo apt-get install openssh-server
```

2. install 🐍 python:
```bash
sudo apt-get install python3
```
3. create user for ansible execution

```bash
sudo adduser ansbile
```

```bash
sudo usermod -aG sudo ansible
```
4. copy your local ssh public key to ansible home ssh folder
```bash
# under ansible user
mkdir ".ssh"
```
```bash
# control node
ssh-copy-id ansible@ip
```
