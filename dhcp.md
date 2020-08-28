 yum install dhcp -yyyy
  935  vim /etc/dhcp/dhcpd.conf 
  936  cp /usr/share/doc/dhcp-4.2.5/dhcpd.conf.example /etc/dhcp/dhcpd.conf 
  937  vim /etc/dhcp/dhcpd.conf 
  938  systemctl restart dhcpd
  939  ifconfig
  940  systemctl restart network
  941  ifconfig
  942  ifdown ens33
  943  ifup ens33
  944  ifconfig
  945  ifdown ens33
  946  ifup ens33
