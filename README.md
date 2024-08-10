# Convergent Network Design

![Network](https://drive.google.com/uc?export=view&id=1llv6FHesfGkznQSC_JGzUsRdEYp8TRM-)

Network 1

Data VLAN (VLAN 11)

    Network: 192.168.11.0
    Subnet Mask: 255.255.255.0
    Default Gateway (Static Router IP): 192.168.11.1
    Broadcast Address: 192.168.11.255
    DHCP Server (Static IP): 192.168.11.2
    DNS Server (Static IP): 192.168.11.3
    HTTP Server (Static IP): 192.168.11.4
    DHCP Range for Devices: 192.168.11.5 - 192.168.11.254

Voice VLAN (VLAN 12)

    Network: 192.168.12.0
    Subnet Mask: 255.255.255.0
    Default Gateway (Static Router IP): 192.168.12.1
    Broadcast Address: 192.168.12.255
    DHCP Provided by Server in VLAN 11 (Static IP): 192.168.11.2
    DHCP Range for Voice Devices: 192.168.12.5 - 192.168.12.254

Network 2

Data VLAN (VLAN 21)

    Network: 192.168.21.0
    Subnet Mask: 255.255.255.0
    Default Gateway (Static Router IP): 192.168.21.1
    Broadcast Address: 192.168.21.255
    DHCP Server (Static IP): Configured to serve addresses from 192.168.21.5 to 192.168.21.254
    DHCP Range for Devices: 192.168.21.5 - 192.168.21.254

Voice VLAN (VLAN 22)

    Network: 192.168.22.0
    Subnet Mask: 255.255.255.0
    Default Gateway (Static Router IP): 192.168.22.1
    Broadcast Address: 192.168.22.255
    DHCP Provided by Server in VLAN 21 (Static IP): 192.168.21.2 (assuming a scenario similar to Network 1)
    DHCP Range for Voice Devices: 192.168.22.5 - 192.168.22.254

Network 3

Data VLAN (VLAN 31)

    Network: 192.168.31.0
    Subnet Mask: 255.255.255.0
    Default Gateway (Static Router IP): 192.168.31.1
    Broadcast Address: 192.168.31.255
    DHCP Server (Static IP): Not yet specified, but an example would be 192.168.31.2
    DHCP Range for Devices: 192.168.31.5 - 192.168.31.254

Voice VLAN (VLAN 32)

    Network: 192.168.32.0
    Subnet Mask: 255.255.255.0
    Default Gateway (Static Router IP): 192.168.32.1
    Broadcast Address: 192.168.32.255
    DHCP Provided by Server in VLAN 31 (Static IP): 192.168.31.2 (assuming a scenario similar to Networks 1 and 2)
    DHCP Range for Voice Devices: 192.168.32.5 - 192.168.32.254
