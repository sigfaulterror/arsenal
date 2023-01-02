# HTTP_SCANNER
#plateform/linux #target/remote #cat/RECON #tag/http

## katana - crawl website
This tools will crawl the target website to discover all the possible urls
https://github.com/projectdiscovery/katana
```
katana -u <target> -jc -c 20 -o <output_file>
```

## endpointfinder - look for endpoints inside javascript file
This tool will use regex to search for APIs and endpoint inside a js file
https://github.com/tarunkant/EndPoint-Finder
```
python EndPoint-Finder.py -u <target_js>
```

## kiterunner - bruteforce APIs for frameworks
This tool will try to bruteforce API endpoints instead of classic directory brute force
Check the github page for more routes databases
https://github.com/assetnote/kiterunner
```
kr scan <target> -A apiroutes-210228 -x 20 --ignore-length=1053 --fail-status-codes 403,501,502,426,411
```

## versionshaker - check version of webapp based on git repo
This tool checks the version of a webapp based on the repository of its git project.
It will check files on the local repository with file in the remote webapp
The file list is comma separated list
https://github.com/Orange-Cyberdefense/versionshaker
```
python3 versionshaker.py -c <git_repo> -u <target> -f <files>
```

## jenkins - scan jenkins
This tool will attempt to pull console output, environment variables, and workspaces associated with Jenkins builds. It works both against unauthenticated and authenticated (with creds) servers.
https://github.com/DolosGroup/Jenkins-Pillage
```
jenkins-pillage.py -a <target>
```