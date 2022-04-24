# pihole-compose
Docker compose file for pihole and dns over cloudflare https.

## How-to run

You can setup pihole with encyrpted cloudflare dns by running the below command:

```bash
# replace BIND_IP_ADDRESS value with the hosts IP you wish to bind pihole to,
BIND_IP_ADDRESS="192.168.2.XXX" docker-compose -p pihole up -d
```
