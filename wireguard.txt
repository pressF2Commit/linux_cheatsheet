# import connection - 
nmcli connection import type wireguard file vpnEurope.conf

# autoconnect off - 
nmcli connection modify vpnEurope autoconnect no

# disconnect
nmcli connection down vpnEurope

# connect
nmcli connection up vpnEurope
