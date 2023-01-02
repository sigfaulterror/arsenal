# DNS
#plateform/linux #target/remote #cat/RECON #tag/dns

## dns - aiodnsbrute scanner
DNS scanner using bruteforce
https://github.com/blark/aiodnsbrute
```
aiodnsbrute -w <wordlist_file> -r <resolvers_file> -vv -t <threads> <target>
```

## altdns - permuted subdomain discovery
Altdns is a DNS recon tool that allows for the discovery of subdomains that conform to patterns. Altdns takes in words that could be present in subdomains under a domain (such as test, dev, staging) as well as takes in a list of subdomains that you know of.
https://github.com/infosec-au/altdns
```
altdns -i <discovered_subdomains_file> -o <output_file> -w <permutation_word_list> -r -s results_output.txt
```