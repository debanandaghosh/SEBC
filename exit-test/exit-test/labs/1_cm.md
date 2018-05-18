
root@instance-2 skanduri1987]# cd /etc/yum.repos.d/
vi cloudera-manager.repo 
 
[cloudera-manager]
name = Cloudera Manager, Version 5.11.2
baseurl = https://archive.cloudera.com/cm5/redhat/7/x86_64/cm/5.11.2/
gpgkey = https://archive.cloudera.com/redhat/cdh/RPM-GPG-KEY-cloudera
gpgcheck = 1


yum install cloudera-manager-daemons cloudera-manager-server
