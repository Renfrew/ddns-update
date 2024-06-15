# ddns-update

Scripts to update the DNS records

Dependencies: `jq`, `dig`, `curl`

**Notes**: IPv4 only

The script will log to `/var/log/me.renfrew.dnsUpdate.log` and `/var/log/me.renfrew.dnsUpdate.err`

## Usage

`cloudflare-ddns.sh <ACCESS_TOKEN> <DOMAIN> <SUBDOMAIN> <TTL>`

### Example

`cloudflare-ddns.sh aCcEFfdsOKeN example.com local 300`

## Sample cron job

`*/15 * * * * /Users/renfrew/bin/dns-update sample-token example.me www 3600`
