# what is ipctl
ipctl is an easy IPv6 services address management script
ipctl make use of dns service to get the IPv6 address from the name of the machine
ipctl do not work with IPv4 address

# how to install it
move ipctl into `/usr/bin`, then change owner and rights:
```bash
chmod 755 /usr/bin/ipctl
chown root:root /usr/bin/ipctl
```
# how to use it
## Getting help
without any parameter, ipctl will display the help message

## Listing addresses
the command `ipctl list` will list ethernet cards, vlan ports and network bridges with their respectives interface number and current assigned addresses.

## Adding an address
to add an IPv6 address by its dns name, you just need the name and the port number: `ipctl add www.mydomain.com to 2`

## Removing an address
removing an address is as easy as adding one: `ipctl del www.mydomain.com from 2`
