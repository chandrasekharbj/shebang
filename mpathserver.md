 fdisk /dev/sdd
  915  partprobe /dev/sdd
  916  pvcreate /dev/sdd1
  917  vgcreate sands /dev/sdd1
  918  vgdisplay sands
  919  lvcreate -n lv1 -L +4G sands 
  920  lvdisplay /dev/sands/lv1 
  921  targetcli
  922  systemctl restart target.service 
  923  systemctl enable target.service 
  924  firewall-cmd --permanent --add-service=iscsi-target 
  925  firewall-cmd --reload
  926  firewall-cmd --permanent --add-port=860/tcp
  927  firewall-cmd --reload
  928  netstat -tulnp | grep 3260
  929  systemctl restart target.service 
  930  firewall-cmd --permanent --add-service=iscsi-target 
  931  firewall-cmd --reload
