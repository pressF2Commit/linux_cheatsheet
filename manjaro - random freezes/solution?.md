install these
```bash
yay -S disable-c6-systemd
sudo modprobe msr
```
edit this file:
```bash
sudo nano /etc/modules-load.d/modules.conf
```
add the following line to the end of the file:
```bash
msr
```
reboot computer, enter the following command:
```bash
sudo systemctl enable disable-c6.service
sudo systemctl start disable-c6.service
```