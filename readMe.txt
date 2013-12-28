********************************************************************************
* 
* Drew Limm
* dtl2119
*
********************************************************************************


For my program, I have three java files: Server, Client, and AcceptClient.
When Server.java is executed, it continuously listens to accept clients.
Once a client connects through a socket, a new AcceptClient thread is created
for that user.  

How to run my program:
Server takes 1 parameter, the port number
Client takes 2 parameters, args[0]=ip, args[1]=port number

ex:
>make
>java Server 4119
>java Client localhost 4119


From then on, you will be able to use the three commands:
1)whoelse
2)wholasthr
3)broadcast "message"

for the broadcast command, omit the quotes.  Here is an example:
broadcast Hello All Clients!


Also, keep in mind that I have a file called userlist.txt.  When running the
Server, it grabs that file and creates a 2D array where col1 is username and
col2 is password.  Therefore, to add more authorized users to the server, you
could add more to the userlist.txt file.  The format is username password (with
a space in between).  For example:

Computer science

This would create the user Computer with the password science.
