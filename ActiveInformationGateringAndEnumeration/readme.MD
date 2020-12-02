##Scanning##
>_ Ping

ping scanme.nmap.org

Layer 2 - ARP, 3 -ICMP, 4 -TCP/UDP
>_ nmap
>_nmap  -sn scanme.nmap.org --packet-trace

Port Scaning and Service Enumeration

>_ nmap scanme.nmap.org

Port 22, 113, 139

>_ nmap -p22,113,139 scanme.org

>_ nmap -p22,25,80,113,139,1900 scanme.org -d --packet-trace

>_ nmap scanme.nmap.org -sV
>_ nmap scanme.nmap.org -p22 -A

##Enumerating#
#smb# (samba)

>_ nmap RemoteIp -A




