 vim /etc/rsyslog.cong
  808  vim /etc/rsyslog.conf
  809  systemctl restart rsyslog
  810  vim /etc/logrotate.conf 
  811  man logrotate
  812  cd /var/log
  813  cat secure | grep chan
  814  cat secure | grep password change
  815  cat secure | grep passwo
  816  cat secure | grep naruto
  817  cat secure | grep logical
  818  journalctl _UID=1027
  819  journalctl _UID=0
  820  su - naruto
  821  journalctl _UID=1027
  822  journalctl _UID=1027 --since today
  823  journalctl _UID=0 --since today
  824  journalctl -u vsftpd
  825  journalctl -u firewalld
  826  journalctl -u sshd
  827  journalctl -b
  828  journalctl -b --since today
  829  cd ..
  830  cd  log
  831  cd  audit/
  832  ls
  833  vim audit.log 
  834  cat audit.log | grep selinux
  835  cat audit.log | grep naruto
  836  cat audit.log | grep hinata
  837  cat /var/log/messages | grep naruto
  838  cat /var/log/messages | grep hinata
  839  cat /var/log/messages | grep boot
  840  auditctl -w /etc/passwd -p wra -k passwd
  841  su - naruto 
  842  cat audit.log | grep passwd
  843  man auditctl 
  844  vim /etc/rsyslog.conf 
  845  systemctl restart rsyslog.service 
  846  logger "test from the logserver"
  847  tail /var/log/messages
  848  vim /etc/rsyslog.conf 
  849  systemctl restart rsyslog.service 
  850  logger "test from the logserver"
  851  tail /var/log/messages
  852  vim /etc/rsyslog.conf 
  853  iptables -F
  854  logger "test from the logserver"
  855  cd /var/log
  856  ls
  857  cat messages | grep ldap
  858  cat secure | grep ldap
  859  cat secure | grep slapd
  860  cat messages | grep slapd
  861  cat messages | grep naruto
  862  cd audit/
  863  cat audit.log | grep ldap
  864  cat audit.log | grep naruto
  865  cd
  866  cat messages | grep naruto
  867  cd /var/log
  868  cat messages | grep naruto
  869  vim /etc/rsyslog.conf 
