# C Socket Programming: Private Chat Application
A low-level networking project built to explore TCP/IP stack, C Socket Programming, and Client-Server Architecture. 
<br>
This project implements a bidirectional, offline chat system where a Server and a  Client can exchange secure messages.
<br>
# 🎯 Learning Objectives
Network Fundamentals:  Understanding the life cycle of a socket (Socket → Bind → Listen → Accept → Connect). * C Programming: Deepening knowledge of pointers, buffers, and system calls like read(), write(), and bzero().
<br>
Systems Architecture: Implementing a synchronous messaging protocol between two distinct processes.
# 📂 Project Structure
server.c: The backbone of the system. It listens for incoming connections and manages the communication flow.
<br>
client.c: The interface used to connect to the server via a specific IP address and port number.
# 🛠️ How it Works
The communication follows a strict TCP Handshake and data exchange flow:
<br>
Server side: Opens a socket and waits (listen) on a user-defined port.
<br>
Client side: Requests a connection using the server's hostname/IP and the same port.
<br>
Establishment: The server accepts the connection, creating a dedicated communication channel (newsockfd).
<br>
Messaging: Both parties use read() and write() to exchange strings until the keyword "Bye" is detected.
# 📺 Demonstration
Check out the live demo of the communication between the Client and Server here:
https://youtu.be/nWdoF6Spq5A
