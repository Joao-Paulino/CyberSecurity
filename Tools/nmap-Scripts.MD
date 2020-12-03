
sudo git clone https://github.com/vulnersCom/nmap-vulners.git 

[Optional] sudo ln -s `pwd`/nmap-vulners /usr/share/nmap/scripts/nmap-vulners

>_ sudo nmap --script vulscan/vulscan.nse -sV -p80 192.168.50.171


sudo git clone https://github.com/scipag/vulscan.git

[Optional] sudo ln -s `pwd`/vulscan /usr/share/nmap/scripts/vulscan

>_ udo nmap --script vulscan/vulscan.nse -sV -p80 RemoteHostIp

