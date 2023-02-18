# Minitalk
The 42-minitalk project is a simple implementation of the Minitalk protocol consisting of two different programs. Communication between the two programs is achieved using UNIX signals.

The first part of the project involves writing the "client" program that sends messages. The client program sends messages to the "server" program with a Process ID (PID) number chosen by the user. These messages are encoded using the Minitalk protocol and sent using UNIX signals.

The second part of the project involves writing the "server" program that receives messages. The server program first receives a PID from the client program and then receives messages based on that PID. The server program decodes the messages using the Minitalk protocol and prints them to the screen.

The 42-minitalk project uses the Minitalk protocol to ensure reliable communication between the two programs. The Minitalk protocol encodes messages using a sequence of bits, each of which is either 0 or 1, and sends them using UNIX signals. This method takes precautions against various errors to ensure data security.

The main goal of the project is to help students develop practical skills in system programming, network programming, and data structures.

# Usage
Minitalk can operate in two different modes: server and client. To use the server mode, run the following command:
```
./server
```
This command starts the server mode and displays the PID of the server on the screen. This PID is required to start the client mode.

To start the client mode, run the following command:

```
./client [server PID] [message]
```
Replace [server PID] with the PID displayed by the server and [message] with the message you want to send to the server. The client mode sends the message to the server, which then displays it on the screen.

Installation
To install Minitalk, clone the project repository and compile the code using the following command:

```
make
```
This command compiles the source code and generates the executable files for both the server and client modes.

