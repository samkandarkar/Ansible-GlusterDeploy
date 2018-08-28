Role Name
=========

Ansible-GlusterDeploy is an Ansible Galaxy to configure a 3 node gluster storage cluster . 

Requirements
------------

This is a project which helps you to configure a 3 node cluster of gluster storage. <br>
Prerequisits :<br>
Gluster should be installed in each node of same version.
Systems should be in the same netwrok.

Role Variables
--------------
In the vars file in /vars/main.yml there are some variables whcih users can change or define according to their use case :
Example: 
 # Enter the disk name you have in your nodes (ex. /dev/sdb)
    disk_name: /dev/sdb
    
 # Name the volume group you want to create under the physical volume
    volume_group: vg1

 # Create a thinpool under the volume group
    pool: pool1

 # Mention the size of the thinpool with respect to the size of VolumeGroup
    pool_size: 6g

 # Create a logical volume under the thinpool
    logical_volume: lv

 # Mention the size of logical volume
    lv_size: 200m

 # Name of the brick where the logical volume will be mounted ( This directory will be created on "/" folder. If you want create it on anouther folder then just don't mention "/" .  )
    mount_point_1: brick1

 # IP address of the master 
    master: 192.168.122.60

 # IP of the node1 
    node1: 192.168.122.70

 # IP of the node2
    node2: 192.168.122.80

 # Name of the gluster volume
    volume: vol_name

 # name of the sub directory for the brick (It will create a folder under the mount point)
    sub_dir: subdir

License
-------
GNU General Public License

Author Information
------------------
Shriya Mulay ( mulayshriya@gmail.com ) <br>
Sameer Kandarkar ( samkandarkar@gmail.com )
