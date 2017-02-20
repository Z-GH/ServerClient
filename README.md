# ServerClient
Create Server &amp; Client .Net using TCP to comunicate

/////////////////////////
// ** Author Z ** //
// **       -2017-02-19         ** //
This Project about having a server Console Application, which will receive connections from Client side
Client will send multi messages and expected answers for each

This project been created with .Net Framework 4.5.2

////////
To run it:
First run "ServerClient.exe" and then run "ClientServer.exe"
Once ClientServer gets all the responses back from ServerClient, then it will ask to enter any key to exit.

Handshake:

Client: HELO
Server: HI # Timeout 5 seconds


After a successful handshake the server accepts following commands from the client

Client: COUNT
Server Response: 56 # Integer representing count of successful handshakes


Client: CONNECTIONS

Server Response: 10 # Integer representing the current connections to the server

Client: PRIME

Server Response: 142339 # returns a prime number


Client: TERMINATE

Server Response: BYE # Server terminates the connection


//////
I used TCP comunication to establish a connection with remote endpoint, then we use it to send and receive data. 
That will ensure that the data will be in order

/////
To be improved...

Got the Client side to be control by user, by entering specific data and have multi clients communicate and sending
data at the same time.
