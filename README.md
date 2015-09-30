# Java-TCP-client-server-implementation
Simple client server TCP application. The server uses a hasmap to stores values sent from the client. The client can store and manipulate the data on the server.

The client program takes 1-2 arguments. The first argument is the name or IP address of  the host that the server is running on, and the second (if present) is the port number on which   it’s listening. The second argument defaults to 31357.

The commands that the client can send to the server are

get: key (returns the value stored in the hashmap for that key)

put: key:value (stores the value in the hasmap at the specified key. Drop the previous one if present)

swap: key:key2 (swaps the two value in the hashmap)

remove: key  (removes the key and its value from the hashmap)

get all (returns the content of the hashmap in the form key::value

The server takes two optional command line arguments. The first is the IP address to
which the server’s socket is to be bound. If this is omitted, the server uses the wildcard
address. The second argument is a port number. If no port number is specified, the server
uses port 31357. If the port number is specified, the IP address must also be specified.
