 cryptsetup luksFormat /dev/sdb3
  454  cryptsetup luksOpen /dev/sdb3 chan
  455  mkfs -t xfs /dev/mapper/chan
  456  mkdir /lukchan
  457  mount /dev/mapper/chan /lukchan/
  458  cd /lukchan/
  459  cp /root/Desktop/* .
  460  ls
  461  cd ..
  462  umount /lukchan/
  463  ls
  464  cd lukchan/
  465  ls
  466  mount /dev/mapper/chan /lukchan/
  467  ls
  468  cd ..
  469  cd lukchan/
  470  ls
  471  cd ..
  472  cryptsetup luksClose /dev/sdb3 chan
  473  cryptsetup luksClose  chan
  474  umount lukchan/
  475  cryptsetup luksClose  chan
  476  cd lukchan/
  477  ls
  478  cd ..
  479  cryptsetup luksOpen  chan
  480  cryptsetup luksOpen /dev/sdb3  chan
  481  cd lukchan/
  482  ls
  483  mount /dev/mapper/chan /lukchan/
  484  ls
  485  cd ..
  486  ls
  487  cd lukchan/
  488  ls
  489  cd ..
  490  cryptsetup luksClose chan
  491  vim /etc/fstab
  492  vim /etc/crypttab 
  493  reboot
  494  reboot
  495  vim /root/luks.key
  496  man cryptsetup
  497  cryptsetup luksAddKey /dev/sdb3 /root/luks.key 
  498  cryptsetup luksAddKey /dev/sdb3 /root/luks.key 
  499  vim /etc/crypttab 
