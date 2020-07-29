  cd /var/ftp/pub
  ls
  mkdir packages
  cp -v  /run/media/root/RHEL-7.3\ Server.x86_64/Packages/* ./packages/
  cd packages/
  ls
  createrepo /var/ftp/pub/packages/
  cd /etc/yum.repos.d/
  ls
  vim server.repo 
  systemctl restart vsftpd
  yum repolist
  yum clean all
  yum repolist
  yum update
  systemctl status vsftpd
  yum install yum-plugin-versionlock
  yum versionlock add vsftpd
  yum install kernel -y
  reboot
  cat /etc/redhat-release 
  cat /etc/os-release 
