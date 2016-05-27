### VirtualBox Host-only Networks
vboxnet0:

```
IPv4 Address: 192.168.56.1
IPv4 Network Mask: 255.255.255.0
```

### VirtualBox NAT Networks

```
Network Name: NatNetwork
Network CIDR: 10.0.2.0/24
Network Options: Supports DHCP
```

### Adapter 1

```
Attached to: Host-only Adapter
Name: vboxnet0
```

### Adapter 2

```
Attached to: NAT Network
Name: NatNetwork
```

### eth0

```
DEVICE=eth0
NM_CONTROLLED=no
ONBOOT=yes
BOOTPROTO=static
IPADDR=192.168.56.55
NETMASK=255.255.255.0
```

### eth1

```
DEVICE=eth1
NM_CONTROLLED=no
ONBOOT=yes
BOOTPROTO=dhcp
TYPE=Ethernet
```

