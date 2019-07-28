# Dockerized Internal DNS Infrastructure
Pi-Hole DNS filtering with CoreDNS forwarding to internal authoritative DNS server and DNS-over-TLS forwarding to Quad9.

## Configuration
The following environment variables are required either in a `.env` file or in the shell.

| Environment Variable | Example                               | Description     |
|---                   |---                                    |---              |
| DOMAIN               | example.com                           | Internal domain. |
| PIHOLE_HOSTNAME      | pihole01                              | Hostname of Pi-Hole container. |
| PIHOLE_PASSWORD      | changeme                              | Pi-Hole admin UI password. |
| AUTHORITATIVE_DNS    | 192.168.1.10                          | IP address of internal authoritative DNS server. |
| DNS_INTERFACE_IPV4   | 192.168.1.11                          | Local IP address to bind Pi-Hole DNS. |
| TRAEFIK_ACME_EMAIL   | email@example.com                     | Email address to register with LetsEncrypt |
| CLOUDFLARE_API_EMAIL | email@example.com                     | Cloudflare API account email address |
| CLOUDFLARE_API_KEY   | a3fe0e9b2851c040aa4f4434742647abbfc80 | Cloudflare API account key |
