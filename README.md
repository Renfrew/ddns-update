# ddns-update

Scripts to update the DNS records

The cloudflare script support both the IPv4 and the IPv6.

The netlify script support only the IPv4 and is legacy, please use it with care.

Dependencies: `jq`, `dig`, `curl`

The script will log to `/var/log/me.renfrew.dnsUpdate.log` and `/var/log/me.renfrew.dnsUpdate.err`

## Usage

`cloudflare-ddns.sh <ACCESS_TOKEN> <DOMAIN> <SUBDOMAIN> <TTL>`

### Example

`cloudflare-ddns.sh aCcEFfdsOKeN example.com local 300`

## Sample cron job

`*/15 * * * * /Users/renfrew/bin/dns-update sample-towwwwwken example.me www 3600`
