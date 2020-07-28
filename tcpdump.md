 ifconfig
 
  ping 192.168.91.139
  tcpdump 
  tcpdump -i bond0
  tcpdump -i bond0 -c 5
  tcpdump src port 22 -c 10
  tcpdump dst port 22 -c 10
  tcpdump dst port 22 -c 10 -w client01.pcap
  tcpdump -r client01.pcap 