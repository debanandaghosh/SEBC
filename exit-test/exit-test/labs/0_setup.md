


[root@instance-1 debanandaghosh]# uptime
 02:41:01 up 3 min,  1 user,  load average: 0.02, 0.04, 0.03
[root@instance-1 debanandaghosh]# uptime -p
up 3 minutes



[root@instance-2 debanandaghosh]# uptime -p
up 5 minutes
[root@instance-2 debanandaghosh]# uptime
 02:42:31 up 5 min,  1 user,  load average: 0.00, 0.04, 0.03
[root@instance-2 debanandaghosh]# 


[root@instance-3 debanandaghosh]# uptime 
 02:43:04 up 5 min,  1 user,  load average: 0.00, 0.00, 0.00
[root@instance-3 debanandaghosh]# uptime -p
up 5 minutes



[root@instance-4 debanandaghosh]# uptime
 02:42:45 up 5 min,  1 user,  load average: 0.01, 0.02, 0.02
[root@instance-4 debanandaghosh]# uptime -p
up 5 minutes


[root@instance-5 debanandaghosh]# uptime 
 02:43:17 up 5 min,  1 user,  load average: 0.00, 0.02, 0.02
[root@instance-5 debanandaghosh]# uptime -p
up 5 minutes


Cloud provide-  Google Cloud 
Linux - Centos 7

[root@instance-2 debanandaghosh]# uname -a
Linux instance-2 3.10.0-862.2.3.el7.x86_64 #1 SMP Wed May 9 18:05:47 UTC 2018 x86_64 x86_64 x86_64 GNU/Linux




Name	Zone	Recommendation	Internal IP	External IP	Connect	
 instance-1	us-east1-b		
10.142.0.2
35.196.69.188 
 	
 instance-2	us-east1-b		
10.142.0.3
35.190.161.179 
 	
 instance-3	us-central1-c		
10.128.0.2
35.184.76.141 
 	
 instance-4	us-central1-c		
10.128.0.3
35.232.122.185 
 	
 instance-5	us-west1-b		
10.138.0.2
35.230.55.189 
 	
	
	


[root@instance-5 debanandaghosh]# df -Th
Filesystem     Type      Size  Used Avail Use% Mounted on
/dev/sda1      xfs       100G  1.6G   99G   2% /
devtmpfs       devtmpfs  7.3G     0  7.3G   0% /dev
tmpfs          tmpfs     7.3G     0  7.3G   0% /dev/shm
tmpfs          tmpfs     7.3G  9.4M  7.3G   1% /run
tmpfs          tmpfs     7.3G     0  7.3G   0% /sys/fs/cgroup
tmpfs          tmpfs     1.5G     0  1.5G   0% /run/user/1000



[root@instance-5 debanandaghosh]# sudo bash
[root@instance-5 debanandaghosh]# useradd -u 2500 thanos
[root@instance-5 debanandaghosh]# useradd -u 2600 hulk
[root@instance-5 debanandaghosh]# useradd -u 2700 groot
[root@instance-5 debanandaghosh]# sudo groupadd blackorder
[root@instance-5 debanandaghosh]# sudo usermod -a -G blackorder thanos
[root@instance-5 debanandaghosh]# sudo groupadd avengers
[root@instance-5 debanandaghosh]# sudo usermod -a -G avengers hulk
[root@instance-5 debanandaghosh]# sudo usermod -a -G avengers groot
[root@instance-5 debanandaghosh]# yum repolist enabled



debanandaghosh:x:1000:1001::/home/debanandaghosh:/bin/bash
microsoft:x:1001:1002::/home/microsoft:/bin/bash
thanos:x:2500:2500::/home/thanos:/bin/bash
hulk:x:2600:2600::/home/hulk:/bin/bash
groot:x:2700:2700::/home/groot:/bin/bash





google-sudoers:x:1000:debanandaghosh
debanandaghosh:x:1001:
microsoft:x:1002:
blackorder:x:1003:thanos
avengers:x:1004:hulk,groot
thanos:x:2500:

