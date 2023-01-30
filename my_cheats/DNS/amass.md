# Amass
#plateform/linux #target/remote #cat/RECON #tag/DNS

## Amass - scan domain name
To scan a specific domain name. 

```
amass enum -d <domain-name> -dir <amass-result-dir>
```

## Amass - scan domain name with already found subdomains
To scan the subdomain of a given domain and include already found subdomains that might have been found using bruteforce or other methods.
```
amass enum -d <domain-name> -dir <amass-result-dir> -nf <found-subdomains>
```

# Amass - read results of scan
To read the scan results from result directory
```
amass db -dir <amass-result-dir> -show
```