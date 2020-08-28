 awk -F  '{print $1}' top
 1101  top | awk -F  '{print $1}' 
 1102  man top
 1103  top | awk -F  '{print $4}' 
 1104  top | awk 'BEGIN{FS=" ";OFS=" "}{print $4}' 
 1105  top | awk 'BEGIN{FS=" ";OFS=" "}{print $1}' 
 1106  top
 1107  man awk
 1108  top | awk 'BEGIN{FS=" ";OFS=""}{print $1}' 
 1109  top | awk 'BEGIN{FS=" ";OFS=""}{print $0}' 
 1110  top | awk 'BEGIN{FS=" ";OFS=""}{print $1}' 
 1111  top | awk 'BEGIN{FS=" ";OFS=""}{print $1,$2}' 
 1112  top | awk 'BEGIN{FS=" ";OFS=""}{print $1,$2}' 
 1113  top | awk 'BEGIN{FS=" ";OFS=""}{print $2}' 
 1114  top | awk 'BEGIN{FS=" ";OFS=""}{print $1,$2}' 
 1115  top | awk 'BEGIN{FS=" ";OFS=""}{print $1,$2,$3}' 
 1116  top | awk 'BEGIN{FS=" ";OFS=""}{print $0}' 
 1117  top | awk 'BEGIN{FS=" ";OFS=""}{print $1,$2}' 
 1118  top | awk 'BEGIN{FS=" ";OFS=""}{print $2}' 
 1119  vim array.sh
 1120  sh array.sh 
 1121  vim array.sh
 1122  sh array.sh 
 1123  vim array.sh
 1124  cp /etc/passwd /tmp/passwd
 1125  sed -n 52p /tmp/passwd
 1126  sed -i 's/chan/lilchanlee/g' /tmp/passwd 
 1127  sed -n 50p /tmp/passwd
 1128  sed -n 40p /tmp/passwd
 1129  sed -i 's/lilchanlee/chan/g' /tmp/passwd 
 1130  sed -n 40p /tmp/passwd
 1131  top | sed 's/ //g'
 1132  top | sed 's/ / /g'
 1133  top | grep "^ " | awk {print $1}
 1134  top | grep "^ " | awk '{print $1}'
 1135  top | awk 'BEGIN{FS=" ";OFS=""}{print $1,$2}' 
 1136  sed -i 's/^chan.*bash$/g' /tmp/passwd
 1137  sed -i 's/^chan.*bash$//g' /tmp/passwd
 1138  sed -n 40p /tmp/passwd
 1139  history
[root@client01 tmp]# 
