# DNS
#plateform/linux #target/remote #cat/RECON #tag/dns

## dnsReaper - subdomain takeover
Signature based scanning engine, this tool based on the signature in the signatures directory will detected possible subdomain takeover.
https://github.com/punk-security/dnsReaper
```
python main.py file --filename <target>  --enable-unlikely
```

## dnsReaper - subdomain takeover in cloud
Signature based scanning engine, this tool based on the signature in the signatures directory will detected possible subdomain takeover, the subdomains are fetched using API calls to the cloud provider.
cloud_provider: [aws|cloudflare|azure]
https://github.com/punk-security/dnsReaper
```
python main.py <cloud_provider> --enable-unlikely
```

## dnsReaper - subdomain takeover using zonetransfer
Signature based scanning engine, this tool based on the signature in the signatures directory will detected possible subdomain takeover, the subdomains will be fetched using zonetransfer.
https://github.com/punk-security/dnsReaper
```
python main.py zonetransfer --zonetransfer-nameserver <zonetransfer_nameserver> --zonetransfer-domain <zonetransfer_domain>  --enable-unlikely
```

## dnsReaper - subdomain takeover using bind file
Signature based scanning engine, this tool based on the signature in the signatures directory will detected possible subdomain takeover, the subdomains will be fetched using bind file.
cloud_provider: [aws|cloudflare|azure]
https://github.com/punk-security/dnsReaper
```
python main.py bind --bind-zone-file <bind_zone_file>  --enable-unlikely
```
