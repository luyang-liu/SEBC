### Challenge Setup
```
* cloud provider:AWS
* IP address and NDS name:
   Public :
   IP:172.31.36.244 DNS (IPv4)ec2-34-214-186-29.us-west-2.compute.amazonaws.com  
   IP:172.31.42.244 DNS (IPv4)ec2-54-213-200-112.us-west-2.compute.amazonaws.com
   IP:172.31.40.47 DNS (IPv4)ec2-54-186-0-140.us-west-2.compute.amazonaws.com
   IP:172.31.35.63 DNS (IPv4)ec2-54-202-185-4.us-west-2.compute.amazonaws.com 
   IP:172.31.43.219 DNS (IPv4)ec2-54-202-17-229.us-west-2.compute.amazonaws.com

* Linux release 
   /* cat /proc/version  */
  Linux version 2.6.32-431.el6.x86_64 (mockbuild@c6b8.bsys.dev.centos.org) (gcc version 4.4.7 20120313 (Red Hat 4.4.7-4) (GCC) ) #1 SMP Fri Nov 22 03:15:09 UTC 2013
  
 
 * system capacity for my fist node
   /* df -h*/
[root@ip-172-31-36-244 ~]# df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvde        30G  658M   28G   3% /
tmpfs           7.4G     0  7.4G   0% /dev/shm

                                                   
  * yum repolist
[root@ip-172-31-36-244 ~]# yum repolist enabled
Loaded plugins: fastestmirror, presto
Determining fastest mirrors
 * base: mirrors.unifiedlayer.com
 * extras: linux.mirrors.es.net
 * updates: linux.mirrors.es.net
repo id                                                                                repo name                                                                                         status
base                                                                                   CentOS-6 - Base                                                                                   6,706
extras                                                                                 CentOS-6 - Extras                                                                                    46
updates                                                                                CentOS-6 - Updates                                                                                  756
repolist: 7,508


* List the users&group
`cat /etc/passwd|grep -e reilly -e frankola `

[root@ip-172-31-36-244 ~]# cat /etc/passwd|grep -e reilly -e frankola
reilly:x:2800:500:reilly:/home/reilly:/bin/bash
frankola:x:2900:501:frankola:/home/frankola:/bin/bash

`cat /etc/group|grep -e sanfrancisco -e paloalto `
[root@ip-172-31-36-244 ~]# cat /etc/group|grep -e sanfrancisco -e paloalto
sanfrancisco:x:500:reilly
paloalto:x:501:frankola

```
