# Compose of Nord VPN transmission

## Installation

### Prerequisites

1. Make sure your host has installed `docker`, `docker-compose`
2. You should have NordVPN account

### Install application

Clone directory
```bash
git clone git@github.com:Sherem/vpn-transmission.git
```

Go to project repository
```bash
cd vpn-transmission
```
Install application
```bash
bin/install <installation directory>
```

### Configure application

Modify `.env` file at <installation directory> to set required data:

```dotenv
# NordVpn environment

VPN_USER=<NordVPN user>
VPN_PASS=<NordVPN Password>
# Country to connect
VPN_CONNECT=United_States
VPN_LOCAL_NETWORK=192.168.1.0/25 # Local network

# Transmission environment
TRANSMISSION_DATA=/path/to/transmission
TRANSMISSION_USER=<Transmission interface user>
TRANSMISSION_PASS=<Transmission interface password>
# Timezone
TRANSMISSION_TZ=America/Los_Angeles
```