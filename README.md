# Distributed-Chatroom 
# Description
The program represents a chatroom, which multiple clients can connect to and interact with each other.
There's only a single chatroom, so no addional chatrooms can be created.

# Technical details
Sockets are used, therefore the clients-server architecture is based on tcp.
The server is multithreaded, hence it accepts multiple connections at the same time.
At the start of a client, the user is asked to insert their username. If they're not
registered, the system will automatically register them and allow them right after to interact with the
chatroom.
A user has only a user_name field, so no authentication is required.
If a user is already connected and some client tries to connect with the same username, the server will
ask the client to insert another username.

# Next step
Extend the program with a database that contains users' info and, therefore, allow user registration with 
authentication.
In this part, the program will be tested on different hosts, in order to simulate a distributed environment.
Since now, the program has been tested only on the same host.
