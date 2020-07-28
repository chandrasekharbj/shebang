    cd /run/media/root/RHEL-7.0\ Server.x86_64/
    cd Packages/
    rpm -ivh vsftpd-3.0.2-9.el7.x86_64.rpm 
    cd /var/ftp/pub
    ls
    mkdir Packages
    ls
    cp -v /run/media/root/RHEL-7.0\ Server.x86_64/Packages/* /var/ftp/pub/Packages/
    createrepo /var/ftp/pub/Packages/
    systemctl restart vsftpd
    systemctl enable vsftpd
    cd /etc/yum.repos.d/
    ls
    mv * /tmp/
    vim server.repo
    yum info vsftpd
 