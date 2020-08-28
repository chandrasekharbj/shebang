 iscsiadm -m discovery -t st -p 192.168.91.100:3260
 1035  vim /etc/iscsi/initiatorname.iscsi 
 1036  systemctl restart iscsid
 1037  iscsiadm -m node -T iqn.2020-08.com.example.server:tgt1
 1038  iscsiadm -m node -T iqn.2020-08.com.example.server:tgt1 -p 192.168.91.100:3260 -l
 1039  fdisk -l
 1040  mpathconf --enable
 1041  vim /etc/multipath.conf
 1042  systemctl restart multipathd.service
 1043  multipath -ll
 1044  vim /etc/multipath.conf 
 1045  systemctl restart multipathd.service
 1046  fdisk -l
 1047  ifconfig
 1048  systemctl restart network
 1049  ifconfig 
