# Create a playbook to deploy a webpage using Ansible

## Steps to follow

### Step 1: Install Ansible on your server

```bash
sudo apt update
sudo apt install ansible -y
```
### Step 2: Add an inventory

* Open the Ansible hosts file and add the details:
```bash
vi /etc/ansible/hosts
```
* Add the inventory according to your needs and save it. For example:

```bash
[webservers]
your_server_ip ansible_ssh_user=root ansible_ssh_pass=password
```
### Step 3: Create the YAML file

```bash
touch deploy_webpage.yml
vi deploy_webpage.yml
```

### Step 4: Add the playbook code

* Coppy the sample.yml file from repo

### Step 5: Check the syntax

```bash
ansible-playbook deploy_webpage.yml --syntax-check
```

### Step 6: Run the playbook to deploy on the node

```bash
ansible-playbook deploy_webpage.yml
```
