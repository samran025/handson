SSH
Secure Shell is a protocol which is used for secure remote login

Consists of transport and channel

It consists of
   three major components:

   o  The Transport Layer Protocol [SSH-TRANS] provides server
      authentication, confidentiality, and integrity. it runs over data link layer
      
   o  The User Authentication Protocol [SSH-USERAUTH] authenticates the
      client-side user to the server.  It runs over the transport layer
      protocol.

   o  The Connection Protocol [SSH-CONNECT] multiplexes the encrypted
      tunnel into several logical channels.  It runs over the user
      authentication protocol.






