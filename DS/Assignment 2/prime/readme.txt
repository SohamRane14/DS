Assignment 2
Terminal 1

# complile all the files
idlj -fall ServiceModule.idl
javac *.java ServiceModule/*.java

# start orbd 
orbd -ORBInitialPort 1056

Terminal 2

# start the server
java ServiceServer -ORBInitialPort 1056

Terminal 3
# connect the client
java ServiceClient -ORBInitialPort 1056 -ORBInitialHost localhost