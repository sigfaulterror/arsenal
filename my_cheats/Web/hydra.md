# Hydra
#plateform/linux #target/remote #cat/ATTACK/BRUTEFORCE #tag/http

## hydra - http - form - userlist and password list

This tool will bruteforce http form login and will check the response for the keyword parameter, if based on the mode [S|F](Success|Fail) will mark the login and password as a hit or a miss.

detection_mode: [S|F], S for success (if the keyword is found in the response then it is a hit), F for failure (if the keyword is NOT found in the response then it is a hit) 

```
hydra -L <usernames_file>  -P <passwords_file> <target> http-post-form  "<login_path>:username=^LOGIN^&password=^PASS^:<detection_mode>=<keyword>"
```
## hydra - https - form - userlist and password list

This tool will bruteforce https form login and will check the response for the keyword parameter, if based on the mode [S|F](Success|Fail) will mark the login and password as a hit or a miss.

detection_mode: [S|F], S for success (if the keyword is found in the response then it is a hit), F for failure (if the keyword is NOT found in the response then it is a hit) 

```
hydra -L <usernames_file>  -P <passwords_file> <target> https-post-form  "<login_path>:username=^LOGIN^&password=^PASS^:<detection_mode>=<keyword>"
```