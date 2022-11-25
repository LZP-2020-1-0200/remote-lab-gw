# remote-lab-gw
Attālināta vārteja uz laboratorijas tīkla iekārtām

trail=pogas_gladrewrox

apt update

apt upgrade

hostnamectl set-hostname newhostname

timedatectl list-timezones | grep Riga

timedatectl set-timezone Europe/Riga

nano /etc/systemd/timesyncd.conf
NTP=lv.pool.ntp.org

apt install wpasupplicant

nano /etc/netplan/01-netcfg.yaml

nano /etc/sysctl.conf

https://upcloud.com/community/tutorials/configure-iptables-ubuntu/

iptables --table nat --append POSTROUTING --out-interface wlo1 -s 10.0.0.0/24 -j MASQUERADE

apt install iptables-persistent

https://ubuntu.com/server/docs/network-dhcp

apt install isc-dhcp-server

nano /etc/dhcp/dhcpd.conf

nano /etc/default/isc-dhcp-server

systemctl restart isc-dhcp-server.service

nano /etc/systemd/logind.conf

service systemd-logind restart

touch ~/.hushlogin

curl -s https://install.zerotier.com | bash

zerotier-cli join networkid9abcdef

sudo apt install lamp-server^
