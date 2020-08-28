udevadm /dev/mapperSANDS
 1057  udevadm /dev/mapper/SANDS
 1058  udevadm /dev/SANDS
 1059  udevadm info  /dev/SANDS
 1060  udevadm info  /dev/mapper/SANDS
 1061  cd /bin
 1062  vim deviceadded.sh
 1063  vim deviceremoved.sh
 1064  chmod 755 deviceadded.sh 
 1065  chmod 755 deviceremoved.sh
 1066  cd /etc/udev/rules.d/
 1067  ls
 1068  cat 98-kexec.rules 
 1069  vim 100-net.rules
 1070  udevadm control --reload 
 1071  cd /tmp/
 1072  ls
 1073  ls
 1074  vim /bin/deviceadded.sh 
 1075  touch devicelog.log
 1076  udevadm control --reload 
 1077  ls
 1078  cat devicelog.log 
 1079  cat devicelog.log 
 1080  cat devicelog.log 
 1081  vim /bin/deviceadded.sh 
 1082  vim /etc/udev/rules.d/100-net.rules 
 1083  udevadm control --reload 
 1084  cat devicelog.log 
 1085  cat devicelog.log 
 1086  nmcli device status
 1087  nmcli connection show
 1088  cat devicelog.log 
 1089  nmcli device status
 1090  ifup eno33554992
 1091  dmesg
 1092  dmesg | grep /dev/sd
 1093  ifconfig 
 1094  cat devicelog.log 
 1095  vim /etc/udev/rules.d/100-net.rules 
 1096  udevadm control --reload 
 1097  cat devicelog.log 
 1098  vim /etc/udev/rules.d/100-net.rules 
