 whereis cat
  677  ls -l /bin/cat
  678  ll /etc/passwd
  679  ls -l /sbin/useradd
  680  llc/etc/group
  681  ll /etc/group
  682  cd /
  683  cat /etc/shadow
  684  whereis cat
  685  ll /bin/cat
  686  ll /bin/su
  687  chmod u+s /bin/cat
  688  ll /bin/cat
  689  chmod u-s /bin/cat
  690  ll /etc/shadow
  691  ll /etc/passwd
  692  ll /bin/passwd
  693  chmod u-s /bin/passwd
  694  ll /bin/passwd
  695  chmod u+s /bin/passwd
  696  ll /bin/passwd
  697  cd
  698  ls
  699  l
  700  mkdir proj
  701  ll proj/
  702  ls -l proj/
  703  ls -l proj
  704  ll
  705  chgrp orguser01 proj
  706  ll
  707  chgrp kaipulla proj
  708  cat /etc/passwd
  709  chgrp vadivelu proj
  710  ll
  711  cd proj/
  712  touch f1 f2
  713  ll
  714  cd ..
  715  chmod g+s proj/
  716  cd proj/
  717  touch f2 f3
  718  ll
  719  chgrp -R vadivelu proj
  720  ccccccccccd ..
  721  cd ..
  722  chgrp -R vadivelu proj
  723  cd proj/
  724  ll
  725  passwd vandumurugan 
  726  cd /
  727  mkdir project
  728  ll
  729  chgrp vadivelu project/
  730  ll
  731  chmod g+s project/
  732  ll
  733  cd proj
  734  cd project/
  735  ls
  736  cat > tx
  737  cd ..
  738  chmod 2777  project/
  739  ls
  740  ll
  741  cd project/
  742  touch r1 r2 r3
  743  cd ..
  744  chmod o+t project/
  745  chmod o-r,o-w project/
  746  ll
  747  passwd snakebabu 
  748  cd project/
  749  ls -l
  750  groupmems -g vadivelu -l
  751  passwd soonapana 
  752  ll
  753  cd ..
  754  ll
  755  cd project/
  756  ll
  757  cd ..
  758  getfacl project/
  759  setfacl -m g:vadivelu:r-- project/
  760  getfacl project/
  761  cd project/
  762  ll
  763  getfacl project/
  764  cd ..
  765  getfacl project/
  766  cd project/
  767  ll
  768  getfacl s1
  769  cd ..
  770  getfacl project/
  771  man setfacl
  772  setfacl -d -m g:vadivelu:r-- /project
  773  getfacl project/
  774  cd project/
  775  ll
  776  setfacl -d -x g:vadivelu:r-- /project
  777  setfacl -d -x g:vadivelu /project
  778  getfacl project/
  779  cd..
  780  cd ..
  781  ll
  782  getfacl project/
  783  setfacl -d -x g:vadivelu /project
  784  getfacl project/
  785  man setfacl
  786  setfacl -k -x g:vadivelu /project
  787  getfacl project/
  788  setfacl -m g:vadivelu:r-- /project
  789  getfacl /project/
  790  cd proje
  791  cd project/
  792  man setfacl
  793  cd ..
  794  setfacl -R -m g:vadivelu:r-- /project
  795  getfacl project/
  796  cd project/
  797  ll
  798  ls
  799  ll
  800  setfacl -m u:snakebabu:r-- r1
  801  groupadd vadivelu1
  802  gpasswd -a ayyasamy
  803  gpasswd -a ayyasamy vadivelu1
  804  cat /etc/group
  805  id ayyasamy
  806  gpasswd -M vandumurugan,kaipulla,snakebabu,soonapana vadivelu1
  807  cat /etc/group
  808  cd ..
  809  setfacl -m g:vadivelu1:r-- /project
  810  cd project/
  811  cd ..
  812  mkdir /common/adm
  813  cat /etc/passwd
  814  cat /etc/passwd
  815  cat /etc/group
  816  cd /common/
  817  ll
  818  chgrp admin adm
  819  ll
  820  chmod g+w adm
  821  ll
  822  groupmems -g admin -l
  823  chmod g+s adm
  824  cd adm
  825  ll
  826  ll
  827  cd ../..
  828  ll
  829  chmod o-r,o-x common/
  830  ll
  831  chmod u+w common/
  832  ll
  833  chmod g+w common/
  834  ll
  835  cd /common/adm
  836  ll
  837  cp /etc/fstab /var/tmp/fstab
  838  cd /var/tmp/
  839  ls
  840  getfacl fstab 
  841  setfacl -m u:natasha:rw- /var/tmp/fstab 
  842  setfacl -m u:harry:--- /var/tmp/fstab 
  843  getfacl fstab 
  844  cd /common/adm/
  845  ll
  846  cd ..
  847  ll
  848  chmod o-r,o-x adm
  849  ls
  850  ll
  851  cd /
  852  touch temp.sh
  853  ls
  854  ll temp.sh 
  855  chmod 440 temp.sh
  856  ll temp.sh 
  857  rm -rf temp.sh 
  858  ll /
  859  chmod 777 common/
  860  groupadd proja
  861  useradd -g proja pa1
  862  id pa1
  863  useradd -g proja pa2
  864  useradd -g proja pa3
  865  useradd -g proja pa4
  866  useradd -g proja pa5
  867  groupadd projb
  868  useradd -g projb pb1
  869  useradd -g projb pb2
  870  useradd -g projb pb3
  871  mkdir /home/project
  872  chmod 770 /home/project/
  873  setfacl -m g:proja:rwx /home/project/
  874  setfacl -m g:projb:rwx /home/project/
  875  chmod o+t /home/project/
  876  ll /home/project/
  877  ll /home |grep project
  878  ls /home/project/
  879  ll /home/project/
  880  useradd test
  881  cat /etc/group | grep proja
  882  cat /etc/passwd | grep 1045
  883  cat /etc/passwd | grep 1046

