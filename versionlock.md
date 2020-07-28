    yum install yum-plugin-versionlock -y
    yum versionlock list
    yum versionlock add vsftpd
    yum versionlock list
    yum versionlock delete vsftpd
    yum versionlock list
    yum history list
    yum history info 7
    yum history undo 7
    yum history list
    yum history info 6
    yum    history undo 6
