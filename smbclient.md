  yum install samba-client* -y
  501  smbclient -L //192.168.91.143
  502  smbclient -L //192.168.91.143
  503  smbclient  //192.168.91.143/testsmbshare
  504  ls
  505  smbclient  //192.168.91.143/testsmbshare
  506  ls
  507  cat client01.pcap | more
  508  tcpdump -r client01.pcap 
  509  ls
  510  smbclient  //192.168.91.143/testsmbshare
  511  smbclient -L //192.168.91.143
  512  smbclient -L //192.168.91.143/testsmbshare
  513  smbclient  //192.168.91.143/testsmbshare
  514  smbclient -L //192.168.91.143/testsmbshare -U chan
  515  smbclient -L //192.168.91.143/testsmbshare -U chan
  516  smbclient -L //192.168.91.143/testsmbshare -U chan
  517  smbclient -L //192.168.91.143/testsmbshare -U chan
  518  smbclient -L //192.168.91.143/testsmbshare -u chan
  519  smbclient -L //192.168.91.143/testsmbshare -U chan
  520  smbclient -L //192.168.91.143/testsmbshare -U chan
  521  smbclient  //192.168.91.143/testsmbshare -U chan
  522  smbclient  //192.168.91.143/testsmbshare -U chan
  523  mkdir /sambadata
  524  mount -t cifs -o username=chan,password=chan //192.168.91.143/testsmbshare /sambadata/
  525  cd /sambadata/
  526  ls
  527  df -hT
  528  umount /sambadata/
  529  cd
  530  umount /sambadata/
  531  yum install cifs-utils.x86_64 -y
  532  mount -o username=chan //192.168.91.143/testsmbshare /sambadata/
  533  df -hT
  534  cd /sambadata/




server
yum install samba -y
vim /etc/samba/smb.conf
systemctl restart smb
iptables -F
ls -Zd /common
getsebool -a | grep samba
setsebool -P samba_create_home_dirs=1
setsebool -P samba_create_domain_controller=1
setsebool -P samba_enable_home_dirs=1
setsebool -P samba_export_all_ro=1
setsebool -P samba_export_all_rw=1


vim /etc/samba/smb.conf
smbpasswd -a chan
systemctl restart smb
