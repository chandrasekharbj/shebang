 lvdisplay /dev/vg1/lv111
  400  lvdisplay /dev/vg1/lv1
  401  lvextend -L +200M /dev/vg1/lv1
  402  xfs_growfs /dev/vg1/lv1
  403  df -hT
  404  yum install xfsdump -y
  405  ls /lv1data/
  406  cp /root/Desktop/* /lv1data/
  407  ls /lv1data/
  408  xfsdump -f /tmp/lv1data.dump /lv1data
  409  umount /lv1data/
  410  lvreduce -L 200M /dev/vg1/lv1
  411  mkfs -t xfs /dev/vg1/lv1
  412  mkfs.xfs -f /dev/vg1/lv1
  413  mount /dev/vg1/lv1 /lv1data/
  414  ls /lv1data/
  415  ls /tmp
  416  xfsrestore -f /tmp/lv1data.dump /lv1data/
  417  ls /lv1data/
  418  df -hT
  419  lvdisplay /dev/vg1/lv1
  420  lvextend -L 300M /dev/vg1/lv1
  421  xfs_growfs /dev/vg1/lv1
  422  df -hT
  423  lvextend -L 500M /dev/vg1/lv1
  424  xfs_growfs /dev/vg1/lv1
  425  df -hT
  426  pvdisplay
  427  fdisk -l
  428  fdisk /dev/sdc
  429  partprobe /dev/sdc
  430  pvcreate /dev/sdb9
  431  pvcreate /dev/sdc9
  432  vgextend vg1    /dev/sdc9
  433  vgdisplay vg1
  434  vgreduce vg1 /dev/sdc9
  435  vgdisplay vg1
  436  vgextend vg1    /dev/sdc9
  437  vgdisplay vg1
  438  df -hT
  439  fdisk /dev/sdc
  440  fdisk /dev/sdc
  441  partprobe /dev/sdc
  442  pvcreate /dev/sdc10
  443  vgcreate -s 16M cgi /dev/sdc10
  444  vgdisplay cgi
  445  lvcreate -n lv1cgi -L +500M cgi
  446  lvdisplay /dev/cgi/lv1cgi 
  447  lvremove /dev/cgi/lv1cgi 
  448  vgremove cgi 
  449  vgdisplay cgi
  450  pvremove /dev/sdc10
  451  fdisk -l
  452  df -hT
  453  lvdisplay /dev/vg1/lv1 
  454  fdisk /dev/sdc
  455  fdisk -l
  456  fdisk /dev/sdb10
  457  fdisk /dev/sdb
  458  partprobe /dev/sdb
  459  pvcreate /dev/sdb10
  460  vgextend vg1                /dev/sdb10
  461  lvextend -L +300 /dev/vg1/lv1
  462  xfs_growfs /dev/vg1/lvl
  463  df -hT
  464  lvremove /dev/vg1/lv1
  465  xfs_growfs /dev/vg1/lv2
  466  df -hT
  467  lvremove /dev/vg1/lv1
  468  vim /etc/fstab 
  469  lvremove /dev/vg1/lv1
  470  lvremove /dev/vg1/lv2
  471  man lv
  472  lvremove -f /dev/vg1/lv2
  473  umount /lv1data/
  474  lvremove /dev/vg1/lv1
  475  umount /lv2data/
  476  lvremove /dev/vg1/lv2
  477  vgdisplay vg1
  478  pvdisplay 
  479  vgremove vggggggggg1
  480  vgremove vg1
  481  pvdisplay 
  482  pvremove /dev/sdb10
  483  pvremove /dev/sdb9
  484  pvremove /dev/sdb8
  485  pvremove /dev/sdc9
  486  pvdisplay 
  487  fdisk /dev/sdb
  488  partprobe /dev/sdb
  489  fdisk /dev/sdc
  490  df -hT
  491  fdisk /dev/sdc
  492  partprobe /dev/sdc
  493  reboot
  494  su - chan
  495  su - chan
  496  fdisk | grep /dev/null
  497  fdisk -l | grep /dev/null
  498  fdisk -l | grep /dev/sdc
  499  init 0
  500  fdisk -l | grep /dev/sdd
  501  fdisk -l | grep /dev/sde
  502  fdisk -l | grep /dev/sdf
  503  fdisk /dev/sdd
  504  partprobe /dev/sdd
  505  fdisk /dev/sde
  506  partprobe /dev/sde
  507  mkfs -t xfs /dev/sde1
  508  df -h
  509  fdisk -l
  510  mkdir /sde1data
  511  mount /dev/sde1 /sde1data/
  512  vim /etc/fstab 
  513  df -h
  514  pvcreate /dev/sdd1
  515  pvcreate /dev/sdf
  516  vgcreate vg1 /dev/sdd1 /dev/sdf
  517  vgdisplay vg1
  518  vgremove vg1
  519  vgcreate VGRLL /dev/sdd1 /dev/sdf
  520  vgremove VGRLL 
  521  vgcreate VGRLL /dev/sdd1 /dev/sdf
  522  vgdisplay VGRLL 
  523  lvcreate -n LVsmall -L 200M VGRLL 
  524  lvcreate -n LBbig -L 600M VGRLL 
  525  mkfs -t xfs /dev/VGRLL/LVsmall
  526  mkdir /lvsmall
  527  mount /dev/VGRLL/LVsmall /lvsmall/
  528  mkfs -t xfs /dev/VGRLL/LBbig
  529  mkdir /lbbig
  530  mount /dev/VGRLL/LBbig /lbbig/
  531  df -h
  532  vim /etc/fstab 
  533  lvextend -L +100M /dev/VGRLL/LVsmall 
  534  xfs_growfs /dev/VGRLL/LVsmall 
  535  df -h
  536  history
