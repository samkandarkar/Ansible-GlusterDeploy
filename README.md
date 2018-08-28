# Ansible-GlusterDeploy
Using this repo you can configure a three node cluster of Gluster storage in your environment using Ansible automation tool.

 Prerequisits :
Gluster should be Installed on each node in your environment. You can refer following repository
# For centos :
http://download.gluster.org/pub/gluster/glusterfs/LATEST/CentOS/glusterfs-epel.repo
# For Fedora
http://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm

# 
# Clone this repo to your master node.
 git clone https://github.com/samkandarkar/Ansible-GlusterDeploy.git

# Edit the inventory file
 [nodes] <br>
 IP1 (Can be master's IP) <br>
 IP2 <br>
 IP3
 
 [master] <br>
 Master_IP

