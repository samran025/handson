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
      

Architecture

Host key: each host has atleast one host key. host key is used dureing key exchange to verify that the
   client is really talking to the correct server 
   
 Message Numbers

   SSH packets have message numbers in the range 1 to 255.  These
   numbers have been allocated as follows:

   Transport layer protocol:

      1 to 19    Transport layer generic (e.g., disconnect, ignore,
                 debug, etc.)
      20 to 29   Algorithm negotiation
      30 to 49   Key exchange method specific (numbers can be reused
                 for different authentication methods)

   User authentication protocol:

      50 to 59   User authentication generic
      60 to 79   User authentication method specific (numbers can be
                 reused for different authentication methods)

   Connection protocol:

      80 to 89   Connection protocol generic
      90 to 127  Channel related messages

   Reserved for client protocols:

      128 to 191 Reserved

   Local extensions:

      192 to 255 Local extensions   
      
      
  The connection protocol [SSH-CONNECT] specifies a mechanism to
   multiplex multiple streams (channels) of data over the confidential
   and authenticated transpor






