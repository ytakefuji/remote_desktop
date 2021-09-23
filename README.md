# remote_desktop
<pre>
$ sudo apt update && sudo apt upgrade 
$ sudo apt install tasksel 
$ tasksel
  picking Ubuntu desktop
$ sudo systemctl set-default graphical.target 

$ sudo apt install xrdp
$ sudo systemctl status xrdp
$ sudo usermod -a -G ssl-cert xrdp 
$ sudo vi /etc/xrdp/startwm.sh 
  adding two lines before test command:
Unset DBUS_SESSION_ADDRESS
Unset XDG_RUNTIME_DIR
$ sudo ufw allow from 192.168.1.0/24 to any port 3389 
$ sudo ufw reload

for accessing the remote site:
run the remote access software
Session Xorg
username ...
passwd ...
</pre>
