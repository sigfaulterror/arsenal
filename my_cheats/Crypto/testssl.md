# tls
#plateform/linux #target/remote #cat/RECON #tag/crypto

## testssl - rapid tls scan of server
testssl.sh is a free command line tool which checks a server's service on any port for the support of TLS/SSL ciphers, protocols as well as recent cryptographic flaws and more.
https://testssl.sh/
```
./testssl.sh <target>
```
## sslsplit  - mitm ssl proxy 
#cat/ATTACK/MITM
capture packet using iptables rules and send it to sslsplit to for mitm. 
https://www.roe.ch/SSLsplit
packet capture documentation: https://kaisenlinux.org/manpages/sslsplit.html
```
sslsplit -X capture.pcap -M keyfile.log -S logdir/  -k ca.key -c ca.crt -D ssl <listen_ip> <listen_port> tproxy
```