### Challenge Setup
```
* cloud provider:AWS
* IP address and NDS name:
   Public :
   IP:172.31.40.179 DNS (IPv4)ec2-54-187-226-190.us-west-2.compute.amazonaws.com  
   IP:172.31.42.112 DNS (IPv4)ec2-54-186-60-199.us-west-2.compute.amazonaws.com
   IP:172.31.33.201 DNS (IPv4)ec2-54-201-252-26.us-west-2.compute.amazonaws.com
   IP:172.31.40.19 DNS (IPv4)ec2-54-202-34-49.us-west-2.compute.amazonaws.com  
   IP:172.31.44.80 DNS (IPv4)ec2-54-245-6-153.us-west-2.compute.amazonaws.com

* Linux release 
   /* cat /proc/version  */
  Linux version 2.6.32-431.el6.x86_64 (mockbuild@c6b8.bsys.dev.centos.org) (gcc version 4.4.7 20120313 (Red Hat 4.4.7-4) (GCC) ) #1 SMP Fri Nov 22 03:15:09 UTC 2013
  
 
 * system capacity for my fist node
   /* df -h*/
  $df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvde        30G  656M   28G   3% /
tmpfs           7.4G     0  7.4G   0% /dev/shm

                                                   
  * yum repolist
Loaded plugins: fastestmirror, presto
base                                                                                                                                                                    | 3.7 kB     00:00     
base/primary_db                                                                                                                                                         | 4.7 MB     00:00     
extras                                                                                                                                                                  | 3.4 kB     00:00     
extras/primary_db                                                                                                                                                       |  29 kB     00:00     
updates                                                                                                                                                                 | 3.4 kB     00:00     
updates/primary_db                                                                                                                                                      | 4.7 MB     00:00     
repo id                                                                                repo name                                                                                         status
base                                                                                   CentOS-6 - Base                                                                                   6,706
extras                                                                                 CentOS-6 - Extras                                                                                    46
updates                                                                                CentOS-6 - Updates                                                                                  756
repolist: 7,508


* List the users&group
`cat /etc/passwd|grep -e jimenez -e beltran`

[root@ip-172-31-40-179 ~]# cat /etc/passwd|grep -e jimenez -e beltran
jimenez:x:2800:500:jimenez:/home/jimenez:/bin/bash
beltran:x:2900:501:beltran:/home/beltran:/bin/bash



`cat /etc/group|grep -e rangers -e astros`
[root@ip-172-31-40-179 ~]# cat /etc/group|grep -e rangers -e astros
rangers:x:500:jimenez
astros:x:501:beltran


```

