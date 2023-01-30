# Server side template injection
#plateform/linux #target/remote #cat/ATTACK/INJECTION #tag/http

## tplmap - scan for template injection

Tplmap is able to detect and exploit SSTI in a range of template engines to get access to the underlying file system and operating system. Run it against the URL to test if the parameters are vulnerable.

https://github.com/epinna/tplmap

```
./tplmap.py -u '<target_url>'
```
## hydra - https - form - userlist and password list

This tool will bruteforce https form login and will check the response for the keyword parameter, if based on the mode [S|F](Success|Fail) will mark the login and password as a hit or a miss.

detection_mode: [S|F], S for success (if the keyword is found in the response then it is a hit), F for failure (if the keyword is NOT found in the response then it is a hit) 

```
hydra -L <usernames_file>  -P <passwords_file> <target> https-post-form  "<login_path>:username=^LOGIN^&password=^PASS^:<detection_mode>=<keyword>"
```