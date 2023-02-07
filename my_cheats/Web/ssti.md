# Server side template injection
#plateform/linux #target/remote #cat/ATTACK/INJECTION #tag/http

## tplmap - scan for template injection

Tplmap is able to detect and exploit SSTI in a range of template engines to get access to the underlying file system and operating system. Run it against the URL to test if the parameters are vulnerable.

https://github.com/epinna/tplmap

```
./tplmap.py -u '<target_url>'
```
