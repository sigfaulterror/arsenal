# HTTP_SCANNER
#plateform/linux #target/remote #cat/RECON #tag/http

## aquatone - rapid scan
#tag/headless_browser
This tools grabs screenshots of multiple hosts and also the responses
https://github.com/michenriksen/aquatone
```
cat <host_list_file> | aquatone 
```

## aquatone - scan specific ports
#tag/headless_browser
This tools grabs screenshots of multiple hosts ports: multiple ports separated by comma 
https://github.com/michenriksen/aquatone

```
cat <host_list_file> | aquatone -ports <ports>
```

## aquatone - scan nmap xml result
#tag/headless_browser
This tools grabs screenshots of multiple hosts, the input is nmap xml scan result 
https://github.com/michenriksen/aquatone

```
cat <nmap_xml_output> | aquatone -nmap
```