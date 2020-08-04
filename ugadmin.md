 useradd user1
  523  passwd user1
  524  cat /etc/passwd
  525  useradd -u 1005 -s /bin/csh -c normalusr -d /home/user02 user2
  526  cat /etc/passwd
  527  userdel user1
  528  cd /hhhhome
  529  cd /home
  530  ls
  531  userdel -r user2
  532  ls
  533  useradd -d /home/user1     -c normalusr -s /bin/csh user1
  534  rm -rf user1
  535  cd /var/spool/mail/
  536  ls
  537  rm -rf user1 
  538  cd /home
  539  useradd -d /home/user1     -c normalusr -s /bin/csh user1
  540  cat /etc/passwd
  541  passwd -l user1
  542  passwd -u user1
  543  passwd user1
  544  cat   /etc/shadow
  545  passwd -l user1
  546  cat   /etc/shadow
  547  passwd -u user1
  548  cat   /etc/shadow
  549  change -l user1
  550  chage -l user1
  551  chage -m 10 -M 30 -W 5 -I 10 -E 12/12/2020 user1
  552  chage -l user1


 cat /etc/group
  572  groupadd vadivelu
  573  useradd -g vadivelu kaipulla
  574  cat /etc/group
  575  useradd -G vadivelu veerabaghu 
  576  useradd -G vadivelu snakebabu
  577  useradd -G vadivelu vandumurugan
  578  cat /etc/group
  579  cat /etc/passwd
  580  useradd soonapana
  581  useradd ayyasamy
  582* 
  583  cat /etc/passwd
  584  usermod -g 1007 soonapana 
  585  id soonapana
  586  id soonapana
  587  useradd -M soonapana,ayyasamy vadivelu
  588  useradd -M soonapana,ayyasamy vadivelu
  589  gpasswd -M soonapana,ayyasamy vadivelu
  590  cat /etc/group
  591  gpasswd -M veerabaghu,snakebabu,vandumurugan vadivelu
  592  cat /etc/group
  593  id soonapana
  594  gpasswd -a soonapana
  595  gpasswd -a soonapana vadivelu
  596  cat /etc/group
  597  man gpasswd
  598  gpasswd -a ayyasamy vadivelu
