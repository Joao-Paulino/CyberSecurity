Monitor Mode

sudo iw dev

sudo ip link set IFACE down

sudo iw IFACE set monitor control

sudo ip link set IFACE up

sudo ip link set wlan0 down

sudo iw wlan0 set monitor control

sudo ip link set wlan0 up

sudo iw dev

Managed Mode

sudo ip link set IFACE down

sudo iw IFACE set type managed

sudo ip link set IFACE up

sudo ip link set wlan0 down

sudo iw wlan0 set type managed

sudo ip link set wlan0 up

Monitor mode using Airmon-ng

sudo airmon-ng

sudo airmon-ng check

sudo airmon-ng check kill

sudo airmon-ng start wlan0

sudo airmon-ng stop wlan0

sudo systemctl start NetworkManager

monitor mode using iwconfig

sudo iwconfig

sudo ifconfig IFACE down

sudo iwconfig IFACE mode monitor

sudo ifconfig IFACE up

sudo ifconfig wlan0 down

sudo iwconfig wlan0 mode monitor

sudo ifconfig wlan0 up

sudo systemctl stop NetworkManager
