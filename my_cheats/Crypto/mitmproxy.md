# mitmproxy
#plateform/linux #cat/ATTACK/MITM

## mitmproxy - intercept traffic
Mitmproxy can decrypt encrypted traffic on the fly, as long as the client trusts mitmproxy’s built-in certificate authority.
https://docs.mitmproxy.org/
```
mitmproxy --listen-port <listen_port> --ssl-insecure --set console_mouse=false --save-stream-file=+<log_file>
```

## mitmproxy - intercept traffic, specify cert for a domain
Mitmproxy can decrypt encrypted traffic on the fly, as long as the client trusts mitmproxy’s built-in certificate authority. for a target domain a specific certificat is used
https://docs.mitmproxy.org/
```
mitmproxy --listen-port <listen_port> --ssl-insecure --set console_mouse=false --save-stream-file=+<log_file> --certs *.<target_domain>=<cert_file>
```

## mitmproxy - intercept traffic, act as reverse proxy
Mitmproxy can decrypt encrypted traffic on the fly, as long as the client trusts mitmproxy’s built-in certificate authority. all incoming traffic is forwareded to target server.
https://docs.mitmproxy.org/

```
mitmproxy --listen-port <listen_port> --ssl-insecure --set console_mouse=false --save-stream-file=+<log_file> --mode reverse:http://<target>:<port>
```