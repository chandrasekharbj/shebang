336  fdisk -l
  337  reboot
  338  fdisk  -l
  339  fdisk    /dev/sdb
  340  partprobe /dev/sdb
  341  k -l
  342  fdisk -l
  343  mkfs -t xfs /dev/sdb1
  344  mkdir /sdb1data
  345  mount    /dev/sdb1 /sdb1data
  346  cd /sdb1data/
  347  ls
  348  cp /root/Desktop/* .
  349  ls
  350  unmount /sdb1data/
  351  ls
  352  cd
  353  unmount /sdb1data/
  354  umount /sdb1data/
  355  cd /sdb1data/
  356  ls
  357  mount /dev/sdb1 /sdb1data/
  358  ls
  359  ls
  360  cd
  361  cd /sdb1data/
  362  ls
  363  vim /etc/fstab 
  

  395  free -m
  396  man free
  397  free -g
  398  fdisk /dev/sdb
  399  partprobe /dev/sdb
  400  swapon /dev/sdb7
  401  mkswap /dev/sdb7
  402  swapon /dev/sdb7
  403  free -m
  404  swapoff /dev/sdb7
  405  free -m

