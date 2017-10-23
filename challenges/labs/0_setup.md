### Challenge Setup
```
* cloud provider:AWS
* IP address and NDS name:
   Public :
   IP:172.31.41.203 DNS (IPv4)ec2-34-210-71-32.us-west-2.compute.amazonaws.com  
   IP:172.31.40.116 DNS (IPv4)ec2-54-202-139-242.us-west-2.compute.amazonaws.com
   IP:172.31.42.219 DNS (IPv4)ec2-34-210-85-226.us-west-2.compute.amazonaws.com
   IP:172.31.40.143 DNS (IPv4)ec2-34-214-106-121.us-west-2.compute.amazonaws.com
   IP:172.31.40.9 DNS (IPv4)ec2-54-202-132-53.us-west-2.compute.amazonaws.com

* Linux release 
   /* cat /proc/version  */
  Linux version 2.6.32-431.el6.x86_64 (mockbuild@c6b8.bsys.dev.centos.org) (gcc version 4.4.7 20120313 (Red Hat 4.4.7-4) (GCC) ) #1 SMP Fri Nov 22 03:15:09 UTC 2013

 
 * system capacity for my fist node
   /* df -h*/
  $df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvde        30G  669M   28G   3% /
tmpfs           3.7G     0  3.7G   0% /dev/shm


                                                   
  * yum repolist
yum repolist enabled
Loaded plugins: fastestmirror, presto
base                                                                                                                                                                    | 3.7 kB     00:00     
base/primary_db                                                                                                                                                         | 4.7 MB     00:01     
extras                                                                                                                                                                  | 3.4 kB     00:00     
extras/primary_db                                                                                                                                                       |  29 kB     00:00     
updates                                                                                                                                                                 | 3.4 kB     00:00     
updates/primary_db                                                                                                                                                      | 4.7 MB     00:00     
repo id                                                                                repo name                                                                                         status
base                                                                                   CentOS-6 - Base                                                                                   6,706
extras                                                                                 CentOS-6 - Extras                                                                                    46
updates                                                                                CentOS-6 - Updates                                                                                  722
repolist: 7,474

```
@mfernest: Test user/group assignments are missing.
