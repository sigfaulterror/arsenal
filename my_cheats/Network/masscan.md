# masscan

#plateform/linux #target/remote #cat/RECON #tag/scan

## masscan - specific port
```
masscan -p <port> <ip> -e <dev> --rate=1000 -oB masscan_result.scan
```
## masscan - full port
```
masscan -p 1-65535 <ip> -e <dev> --rate=1000 -oB masscan_result.scan
```

## masscan - full UDP port
```
masscan -p 1-65535 -pU <ip> -e <dev> --rate=1000 -oB masscan_result.scan
```

## masscan - HTTP/HTTPS banners grabing
```
masscan <ip> -p 80,433 --rate 1000 --banners --open-only\
--http-user-agent "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:67.0) Gecko/20100101 Firefox/67.0"\
-e <dev> -oL "output.txt" 
```

## masscan - convert input file to list format
#plateform/linux #target/local #cat/UTILS
```
masscan --readscan <input-file> -oL <output-file>
```

## masscan - convert input file to grepabale format
#plateform/linux #target/local #cat/UTILS
```
masscan --readscan <input-file> -oG <output-file>
```
## zmap - rapid scan
```
sudo zmap -p <port> <ip> -o zmap_result.csv
```

## zmap - banners grabbing
```
sudo zmap -p <port> <ip> -o zmap_result.csv && cat zmap_result.csv| zgrab2 http -p <port> --user-agent="Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:67.0) Gecko/20100101 Firefox/67.0"  -o banners.json
```

