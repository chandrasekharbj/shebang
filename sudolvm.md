 visudo -f /etc/sudoers
  990  gpasswd -a chan wheel
  991  groupmems -g wheel -l
  992  touch f11
  993  ll
  994  chown orguser01 f11
  995  chmod 700 f11
  996  ll
  997  chgrp orguser01 f11
  998  ll
  999  ll
 1000  ll
 1001  cccccccccccccd /common/
 1002  cd /common/
 1003  ll
 1004  chown orguser02  f11
 1005  ll
 1006  vim /etc/login.defs
 1007  man ll
 1008  man ls
 1009  cd /etc/defaullts
 1010  cd /etc/default/
 1011  ls
 1012  vim useradd
 1013  useradd user123
 1014  vim useradd
 1015  userdel -r user123
 1016  userdel -r user123
 1017  useradd user123
 1018  ls -a
 1019  cd .
 1020  echo $0
 1021  man useradd 
 1022  vim /etc/security/pwquality.conf 
 1023  vim /etc/security/pwquality.conf 
 1024  vim /etc/security/pwquality.conf 
 1025  vim /etc/security/pwquality.conf 
 1026  vim /etc/security/pwquality.conf 
 1027  vim /etc/security/pwquality.conf 
 1028* 
 1029  vim /etc/security/pwquality.conf 
 1030  vim /etc/security/pwquality.conf 
 1031  cd
 1032  fdisk /dev/sdb
 1033  partprobe /dev/sdb
 1034  pvcreate /dev/sdb8 /dev/sdb9
 1035  pvdisplay /dev/sdb8
 1036  vgcreate vg1 /dev/sdb8 /dev/sdb9
 1037  vgdisplay vg1
 1038  lvcreate -n lv1 -L 500M vg1
 1039  lvcreate -n lv2 -L 1G vg1
 1040  lvdisplay /dev/vg1/lv2
 1041  mkfs      -t xfs /dev/vg1/lv1
 1042  mkdir /lv1data
 1043  mount /dev/vg1/lv1 /lv1data/
 1044  mkfs -t xfs /dev/vg1/lv2
 1045  mkdirr /lv2data
 1046  mkdir /lv2data
 1047  mount /dev/vg1/lv2 /lv2data/
 1048  df -hT
 1049  vim /etc/fstab 
 1050  history
