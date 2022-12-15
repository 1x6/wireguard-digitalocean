# WireGuard installer for digitalocean

put in digitalocean "user data" when creating a droplet and then visit the ip to get the config
<video src="https://cdn.discordapp.com/attachments/1048061961121841213/1052938168573382756/Untitled.mp4">

## Requirements

Supported distributions:

- Ubuntu >= 16.04
- Debian >= 10

## Usage

Download and execute the script. Answer the questions asked by the script and it will take care of the rest.

```bash
#!/bin/bash
curl -O https://raw.githubusercontent.com/1x6/wireguard-digitalocean/master/wireguard-install.sh
chmod +x wireguard-install.sh
./wireguard-install.sh
```

It will install WireGuard (kernel module and tools) on the server, configure it, create a systemd service and a client configuration file.

Run the script again to add or remove clients!

## Providers

I recommend these cheap cloud providers for your VPN server:

- Vultr: Worldwide locations, IPv6 support, starting at \$3.50/month
- Digital Ocean: Worldwide locations, IPv6 support, starting at \$4/month
- PulseHeberg: France, unlimited bandwidth, starting at €3/month
