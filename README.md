# AD-HomeLab
Active Directory Lab infrastructure diagram and explanation
![AD Lab](https://github.com/YoojyimMoua/AD-HomeLab/assets/160559826/58f78761-0649-4d71-88ba-cbfa66424f9d)

This Active Directory environment was created for the purposes of strengthening my learning of related concepts and infrastructure design. This environment consists of a Server serving as our Domain Controller (Windows Server 2022) and a Client1 serving as an example client (Windows 10 Pro). 
The Domain Controller has two NICs, one serving as our DHCP and connected to the public Internet and the other serving as our Internal NIC.
The Domain Controller also has a domain (mydomain.com), Remote Access Server (RAS), Network Address Translation and DHCP configured to allow for clients to connect to the internal NIC and gain access to the internet through the DHCP.
The DHCP has been set to contain an IP range from 172.16.0.100 - 172.16.0.200, a Subnet mask of 255.255.255.0, and a DNS of 172.16.0.1. The Gateway was auto configured.
# Populating AD with auto generated users
A PowerShell script was used to populate a USERS organizational unit within the AD domain. Script and text file of generated user names in separate location.
