# Jenkins and Ansible demo repos

### Objective


### Preriquisite
1. Jenkins host

### Azure hosted Jenkins Master on Ubuntu 

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2F101-jenkins%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2F101-jenkins%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

This template allows you to host an instance of Jenkins on a DS1_v2 size Linux Ubuntu 16.04 LTS VM in Azure.

2. fetch repos
```
git clone https://github.com/sasukeh/Jenkins-ansible-demo.git
```

2. Install ansible on Jenkins host
```
$sudo apt install -y libssl-dev python3-dev python3-pip
$sudo pip3 install ansible
$sudo pip3 install -U cryptgraphy 
```

3. Prep Inventory
```
$vi Jenkins-ansible-demo/Inventory/hosts
```

```
[remote]
192.168.11.11
192.168.11.12
xxx.xxx.xxx.xxx
```

4. Prep Variable file
```
$vi Jenkins-ansible-demo/remote_vmss_var.yml
```

```remote_vmss_var.yml
---

```

5. Prep playbook
```
$vi Jenkins-ansible-demo/ansible_artifact.yml
```

```
---

```

6. run ansible playbook
```
git clone git@github.com:sasukeh/Jenkins-ansible-demo.git
```
7. Configuring Jenkins Job
