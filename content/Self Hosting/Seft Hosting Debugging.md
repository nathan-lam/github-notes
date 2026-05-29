



# Cannot connect to server

There are several reason why you cannot connect to a server

## Check if the ip address changed
- This can happen if the server restarted or change connection to the internet
- These need to be updated
	- The listed ipv4 used for port forwarding
		- the router needs to know which machine the port is for
	- The A record of private ipv4 used by domain


## Allow the port through the firewall
```bash
sudo ufw allow <port>/tcp
sudo ufw allow <port>/udp
```

## Meshnet wifi is not local
If there is a meshnet wifi set up, you cannot connect ot the server if you are on the meshnet and the server is not. Communication needs to be on the same level.


# Unknown 
Solutions that have worked in the past but is not know why
- Being disconnected from your VPN
	- seems to be that I cannot connect to the domain on the local network.

