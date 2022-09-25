* kodibox(moved to pia): only need munin-temperature, with pip3 install temperusb
[munin-temperature]
user root

* hp(moved to pi4): need /etc/munin/plugins/temper_, /etc/munin/munin-node.conf to switch user to root, /usr/share/munin/plugins/temper.py

sudo apt-get install python3-serial
sudo cp temper_ /etc/munin/plugins/temper_0
sudo cp temper.py /usr/share/munin/plugins/temper.py
sudo vi /etc/munin/plugin-conf.d/munin-node

[temper_*]
user root
