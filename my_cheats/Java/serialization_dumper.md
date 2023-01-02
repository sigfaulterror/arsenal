# SerializationDumper
#plateform/linux #target/local #cat/UTILS #tag/java

## SerializationDumper - deserialize object from hex file
A tool to dump and rebuild Java serialization streams and Java RMI packet contents in a more human readable form, this command will deserialize java object from a hex file to a more human readable format.
https://github.com/NickstaDB/SerializationDumper
```
java -jar SerializationDumper.jar -f <hex_file>
```

## SerializationDumper - deserialize object from bin file
A tool to dump and rebuild Java serialization streams and Java RMI packet contents in a more human readable form, this command will deserialize java object from a bin file to a more human readable format.
https://github.com/NickstaDB/SerializationDumper
```
java -jar SerializationDumper.jar -r <bin_file>
```

## SerializationDumper - rebuild serialized object from template file
A tool to dump and rebuild Java serialization streams and Java RMI packet contents in a more human readable form, this command will rebuild a serialized java object from the in_file.
https://github.com/NickstaDB/SerializationDumper
```
java -jar SerializationDumper.jar -b <in_file> <out_file>
```

