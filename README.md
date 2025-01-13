
# Project Enterprise Network

<br><br>
<p align="center">
  <a href="https://viewer.diagrams.net/?tags=%7B%7D&lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=Project%20Enterprise%20Network.drawio#Uhttps%3A%2F%2Fdrive.google.com%2Fuc%3Fid%3D13lTSOZePRxt04y7qujSliA12VnpWliwS%26export%3Ddownload">
    <img src="/img/EnterpriseNetworkTopology.svg">
  </a>
</p>

## The Network

An Enterprise Data Center of the 192.168.6.32/29 network comprises of a DHCP Server, an Active Directory, and an Apache Web Server, all connected to a virtual switch and the switch is connected to a router. 

An Enterprise Client Network of the 192.168.6.40/29 network comprises of a DHCP Relay and a Windows Client machine, all connected to a virtual switch and the switch is connected to the other end of the router.

 A Linux virtual machine is configured as a router using a mix of static routes and iptables, routing the traffic between the two networks.

Installed essential services like DNS, DHCP, Web on the respective machines, along with Active Directory set up to enforce strict group policies on users. Created a bash script ip.sh to automatically assign a static IP address on boot to the relevant machines.
