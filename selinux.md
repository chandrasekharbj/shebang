  getenforce 
   78  setenforce 1
   79  vim /etc/sysconfig/selinux 
   80  getenforce 
   81  reboot
   82  getenfore
   83  getenforce 
   84  setenforce 1
   85  getenforce 
   86  ls
   87  touch f1
   88  ls -Z f1
   89  chcon -t nfs_t f1
   90  ls -Z f1
   91  restorecon f1
   92  ls -Z f1
   93  semanage login -l
   94  cd /
   95  ll
   96  vim /etc/sysconfig/selinux 
   97  cd
   98  ls
   99  chcon -t nfs_t f1
  100  ls -Z
  101  restorecon f1
  102  ls -Z f1
  103  vim /etc/sysconfig/selinux 
  104  setenforce 1
  105  getenforce 
  106  getsebool -a
  107  getsebool | grep ftp
  108  getsebool -a | grep ftp
  109  setsebool ftpd_full_access=1
  110  getsebool -a | grep ftp
  111  setsebool ftpd_full_access=0
  112  getsebool -a | grep ftp
  113  setenforce 0
  114  getenforce 
  115  getsebool -a
  116  setsebool ftpd_full_access=0
  117  setsebool ftpd_full_access=1
  118  getsebool -a | grep ftp
  119  setsebool ftpd_full_access=0
  120  setenforce 1
  121  getenforce 
  122  getsebool -a | grep ssh
  123  getsebool -a | grep sshd
  124  ftp 192.168.91.143
  125  ping 192.168.91.143
  126  yum install ftp -y
  127  ftp 192.168.91.143
  128  ls
  129  ftp 192.168.91.143
  130  ls
  131  cat passwd 
