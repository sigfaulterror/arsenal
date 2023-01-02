# HTTP_SCANNER
#plateform/linux #target/remote #cat/RECON #tag/http

## arjun - http parameter discovery
This tool is for parameters discovery, to run Arjun against a single URL.
https://github.com/s0md3v/Arjun/wiki/Usage

```
arjun -u <target> -t 10
```

## arjun - http parameter discovery
This tool is for parameters discovery, to run Arjun against multiple URLs.
https://github.com/s0md3v/Arjun/wiki/Usage

```
arjun -i <targets_file> -t 10
```

## arjun - http parameter discovery POST method
This tool is for POST parameters discovery, to run Arjun against a single URL.
https://github.com/s0md3v/Arjun/wiki/Usage

```
arjun -u <target> -m POST -t 10
```

## arjun - http json parameter discovery
This tool is for discovering json fields for an API, to run Arjun against a single URL.
https://github.com/s0md3v/Arjun/wiki/Usage
```
arjun -u https://api.example.com/endpoint -m JSON --include='{"root":{"a":"b",$arjun$}}' -t 10
```

## arjun - http xml parameter discovery
This tool is for discovering xml fields for an API, to run Arjun against a single URL.
https://github.com/s0md3v/Arjun/wiki/Usage
```
arjun -u https://api.example.com/endpoint -m XML --include='<?xml><root>$arjun$</root>' -t 10
```