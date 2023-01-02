# cloudbrute
#plateform/linux #target/remote #cat/RECON #tag/cloud

## cloudbrute - storage scan
This Tool will look for storage buckets with a given keyword. The cloud provider is automatically detected, if not detected use specific cloud provider.
https://github.com/0xsha/CloudBrute
```
./CloudBrute  -d <domain> -k <keyword> -a -t 80 -T 100 -w ./data/storage_small.txt
```

## cloudbrute - specific storage scan
This command will bruteforce storage buckets of a specific cloud provider using a given keyword
cloud params can haves these values: [alibaba|amazon|digitalocean|google|linode|microsoft|vultr]
https://github.com/0xsha/CloudBrute
```
./CloudBrute  -d <domain> -k <keyword> -a -t 80 -T 100 -w ./data/storage_small.txt  -c <cloud>
```