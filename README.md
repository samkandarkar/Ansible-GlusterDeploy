# Ansible-GlusterDeploy
Using this repo you can configure a three node cluster of Gluster storage in your environment using Ansible automation tool.

<b> Prerequisits : </b> <br>
For Ansible Deployment all nodes must conatin a passwordless ssh connection from Ansible server and 
Gluster should be Installed on each node in your environment. You can refer following repository
 
 For centos : <br>
 
http://download.gluster.org/pub/gluster/glusterfs/LATEST/CentOS/glusterfs-epel.repo <br>

 For Fedora : <br>
 
http://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm

 
# Clone this repo to your master node.
```
 git clone https://github.com/samkandarkar/Ansible-GlusterDeploy.git
```
# Edit the inventory file
 [nodes] <br>
 IP1 (Can be master's IP) <br>
 IP2 <br>
 IP3
 
 [master] <br>
 Master_IP
 
 # How to play 
 
 To Configure the environment for gluster storage cluster you have to play the file "run.yml" which will invoke Ansible galaxy roles in <b>Ansible-GlusterDeploy</b> folder.<br>
 Before running the playbook , users must change the values in the file "Ansible-GlusterDeploy/vars/main.yml". <br>
 There is example available for configuration of vars file in <b> Ansible-GlusterDeploy/README.md </b>
 
 After doing all configurations releted to your requirement run the followingcommand
 ```
  ansible-playbook run.yml
```
