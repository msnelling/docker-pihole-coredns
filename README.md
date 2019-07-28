# Dockerized Internal DNS Infrastructure
Pi-Hole DNS filtering with CoreDNS forwarding to internal authoritative DNS server and DNS-over-TLS forwarding to Quad9.

## Configuration
The following environment variables are required either in a `.env` file or in the shell.

| Environment Variable | Example                               | Description     |
|---                   |---                                    |---              |
| HOSTNAME             | pihole01                              | Hostname of Pi-Hole container. |
| DOMAIN               | example.com                           | Internal domain. |
| PIHOLE_PASSWORD      | changeme                              | Pi-Hole admin UI password. |
| AUTHORITATIVE_DNS    | 192.168.1.10                          | IP address of internal authoritative DNS server. |
| DNS_INTERFACE_IPV4   | 192.168.1.11                          | Local IP address to bind Pi-Hole DNS. |