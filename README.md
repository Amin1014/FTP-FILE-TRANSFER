A simple python project that shows how to transfer files over a netwrok using ftp.

Server Setup: The server creates a socket and binds it to a specific address and port. It then listens for incoming connections from clients.

Client Setup: Each client creates a socket and connects to the server's address and port.

File Transfer (Upload): Clients read the file they want to send in binary mode and divide it into smaller chunks (if needed). Each client sends these chunks of data to the server over the established socket connection.

File Reception (Server): The server receives the incoming data from multiple clients, reassembles the chunks (if necessary), and saves the file on the server's disk.
