
sudo git clone https://github.com/vulnersCom/nmap-vulners.git
sudo n -s `pwd`/nmap-vulners /usr/share/nmap/scripts/vulnersCom

sudo git clone https://github.com/scipag/vulscan scipag_vulscan
sudo ln -s `pwd`/scipag_vulscan /usr/share/nmap/scripts/vulscan
