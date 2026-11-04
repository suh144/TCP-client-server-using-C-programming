# TCP-client-server-using-C-programming
# Simple Client-Server Distributed Storage

A lightweight, multi-file TCP client-server application written in C using Windows Sockets (Winsock2). Developed as a practical project to explore network programming fundamentals.

## 🛠️ Project Structure
- `server.c`: Listens on a designated TCP port, initializes Winsock, and handles incoming client connections.
- `client.c`: Establishes a socket connection to the server over the local loopback and transmits data.

## 🚀 How to Compile & Run

### 1. Compile using GCC (MinGW)
Open your terminal in the project directory and run the following commands to link the Windows socket library (`-lws2_32`):

```bash
# Compile the Server
gcc server.c -o server.exe -lws2_32

# Compile the Client
gcc client.c -o client.exe -lws2_32
