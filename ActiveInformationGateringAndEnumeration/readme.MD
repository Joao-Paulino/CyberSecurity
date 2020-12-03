##Scanning##
>_ Ping

ping scanme.nmap.org

Layer 2 - ARP, 3 -ICMP, 4 -TCP/UDP

>_ nmap

>_ nmap -sn scanme.nmao.org --packet-tracce

Port Scaning and Service Enumeration
>_ nmap -sn scanme.nmao.org --packet-tracce

>_ nmap scanme.nmap.org

Port 22, 113, 139
>_ nmap -p22,113,139 scanme.org

>_ nmap -p22,25,80,113,139,1900 scanme.org -d --packet-trace

>_ nmap scanme.nmap.org -sV

>_ nmap scanme.nmap.org -p22 -A
>_ nmap -sA -t4 RemoteIp


##Enumerating#
#smb# (samba)

>_ nmap RemoteIp -A

>_ enum4linux -U RemoteIp (user list)

>_ enum4linux -S RemoteIp (shares)

>_ smbclient //RemoteIp/profiles 

##ftp&smtp##

>_ nmap RemoteIp -A

>_ ftp RemoteIp
  name: anonymous (example)
  password: anonymous (example)

#use metasploit framework"
>_ msfconsole

msf>_ use auxiliary/scanner/smtp/smtp_enum

msf auxiliaru(scanner/smtp/smtp_enum) set lhost LocahHostIp

msf auxiliary(scanner/smtp/smtp_enum) set rhost RemoteHostIp

msf auxiliary(scanner/smtp/smtp_enum) show options

msf auxiliary(scanner/smtp/smtp_enum) run

>_ smtp-user-enum.pl -M VRFY /root/list RemoteHostIp  (https://tools.kali.org/information-gathering/smtp-user-enum)

##WebServer&App##
>_ nmap -script=hhtp-eaf-fingerprint RemoteHostIP (https://svn.nmap.org/nmap/scripts/http-waf-fingerprint.nse)

Install wafw00f (The Web Application Firewall Fingerprinting Toolkit)

>_ git clone https://github.com/EnableSecurity/wafw00f.gi

>_ cd wafw00f

>_ sudo python setup.py install

>_ wafw00f -h

>_ wafw00f RemoteHosteIp or  RemoteUrl

>_ nikto -host RemoteHostIp

get DirBuster

>_ git clone https://gitlab.com/kalilinux/packages/dirbuster.git

run

>_ ./DirBuster-1.0-rc.sh

##NetCat##

>_ nc RemoteHostIp RemotePort

#ReverseShell#
>_ nc -nv RemoteIp 4444

>_ nv -lvp 4444

# 7 OSI Layer 
# Physical: coax, Wireless, Hubs, Repeters (Physical Sctructure
# Data Link: Ethernet, PPP, Switech,Bridge (Frames)
# Network: IP, ICMP,IPSec, IGMP (Packets)
# Transport: TCP/UDP (end-To_end Connections)
# Session: API's, Sockets, WinSock (Sync & Send to Port
# Presentation: SSl,SSH IMAP,FTP,MPEG, JPEG (Sytax Lauer)
# Application:HTTP,FTP,IRC,SH,DNS (End User Layer)








  




