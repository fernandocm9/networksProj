# networksProj
Monday Nov 17, 2025 - We have a functioning chat client and chat server which can successfully communicate through a chat protocol. All of the commands except for /quit work, it has logging for server messages, and will quit after 3 minutes of idleness. Things that still don't work/haven't been tested yet are multi-channel, multi-threaded server connection, gracefully shutting down with ctrl-c, and the /quit command working properly. Also there are no colored terminal fonts yet :)


We have created a Chat Server that can handle multiple clients over an internet connection. These clients communicate with the server and accept basic commands that allow for client modifications and personalizations. Beginning with the protocol module, we have the handling for the encoding and decoding of the JSON objects. This is how all of the communication between the client and the server is actually received and sent between each other. This module converts JSON strings to Python modules and vice versa. Objects are sent over sockets, converted into strings, encoded, retrieved from the socket, decoded, and then checked for any whitespaces before or after the data. The line of text is then received over a socket and converted into a Python object. This is how the clients can communicate with the server.
*describe chat server*
*describe chat client*
