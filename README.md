# remote-lab-gw
Attālināta vārteja uz laboratorijas tīkla iekārtām

trail=pogas_gladrewrox

apt install wpasupplicant

nano /etc/netplan/01-netcfg.yaml
nano /etc/sysctl.conf



https://upcloud.com/community/tutorials/configure-iptables-ubuntu/


iptables --table nat --append POSTROUTING --out-interface wlo1 --in-interface enp1s0 -j MASQUERADE

