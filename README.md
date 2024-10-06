# tailscale-qbittorrent-nox

Docker compose configuration for running qBittorrent-nox with Tailscale VPN.

Setup tailscale exit-node anywhere and let torrent run through the specified exit-node.

## Setup

```
export TS_EXTRA_ARGS=--exit-node=100.101.62.82
export TS_AUTHKEY=****
docker compose up
```

## Run

And then access qBittorrent-nox at "http://${created tailscale node}:8080".
Default admin/pw is admin/adminadmin, you can update qbittorrent configuration in web.
