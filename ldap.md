 yum -y install openldap compat-openldap openldap-clients openldap-servers openldap-servers-sql openldap-devel -y
  680  vim /etc/hosts
  681  systemctl restart slapd.service 
  682  netstat -tulnp | grep 389
  683  slappasswd 
  684  cd /etc/openldap/slapd.d/cn\=config/
  685  ls
  686  vim olcDatabase\=\{2\}hdb.ldif 
  687  cd 
  688  cd Desktop/
  689  vim db.ldif
  690  ldapmodify -Y EXTERNAL  -H ldapi:/// -f db.ldif
  691  vim db.ldif
  692  ldapmodify -Y EXTERNAL  -H ldapi:/// -f db.ldif
  693  vim monitor.ldif
  694  ldapmodify -Y EXTERNAL  -H ldapi:/// -f monitor.ldif
  695  cp /usr/share/openldap-servers/DB_CONFIG.example /var/lib/ldap/DB_CONFIG
  696  chown ldap:ldap /var/lib/ldap/*
  697  ldapadd -Y EXTERNAL -H ldapi:/// -f /etc/openldap/schema/cosine.ldif
  698  ldapadd -Y EXTERNAL -H ldapi:/// -f /etc/openldap/schema/nis.ldif 
  699  ldapadd -Y EXTERNAL -H ldapi:/// -f /etc/openldap/schema/inetorgperson.ldif
  700  useradd naruto
  701  passwd naruto
  702  vim base.ldif
  703  ldapadd -x -W -D "cn=ldapadm,dc=example,dc=com" -f base.ldif
  704  vim naruto.ldif
  705  cat /etc/passwd
  706  cat /etc/shadow
  707  vim naruto.ldif
  708  ldapadd -x -W -D "cn=ldapadm,dc=example,dc=com" -f naruto.ldif
  709  ldappasswd -s password123 -W -D "cn=ldapadm,dc=example,dc=com" -x "uid=naruto,ou=People,dc=example,dc=com"
  710  ldapsearch -x cn=naruto -b dc=example,dc=com
  711  firewall-cmd --permanent --add-service=ldap
  712  firewall-cmd --reload 
  713  useradd sasuke
  714  passwd sasuke
  715  cat /etc/passwd
  716  vim sasuke.ldif
  717  vim naruto.ldif 
  718  vim sasuke.ldif
  719  cat /etc/shadow
  720  vim sasuke.ldif
  721  ldapadd -x -W -D "cn=ldapadm,dc=example,dc=com" -f sasuke.ldif
  722  ldappasswd -s password123 -W -D "cn=ldapadm,dc=example,dc=com" -x "uid=sasuke,ou=People,dc=example,dc=com"
  723  ldapsearch -x cn=sasuke -b dc=example,dc=com
  724  ldapsearch -x cn=naruto -b dc=example,dc=com
  725  ldapsearch -x cn=sasuke -b dc=example,dc=com
  726  cat /etc/passwd
  727  vim sasuke.ldif 
  728  ldapadd -x -W -D "cn=ldapadm,dc=example,dc=com" -f sasuke.ldif
  729  ldapmodify -x -W -D "cn=ldapadm,dc=example,dc=com" -f sasuke.ldif
  730  vim sasuke.ldif 
  731  ldapmodify -x -W -D "cn=ldapadm,dc=example,dc=com" -f sasuke.ldif
  732  ldapadd -x -W -D "cn=ldapadm,dc=example,dc=com" -f sasuke.ldif
  733  ldappasswd -s password123 -W -D "cn=ldapadm,dc=example,dc=com" -x "uid=sasuke,ou=People,dc=example,dc=com"
  734  ldapdelete -x -W -D "cn=ldapadm,dc=example,dc=com" -f sasuke.ldif
  735  ldapremove -x -W -D "cn=ldapadm,dc=example,dc=com" -f sasuke.ldif
  736  ldapmodify -x -W -D "cn=ldapadm,dc=example,dc=com" -f sasuke.ldif
  737  vim sasuke.ldif 
