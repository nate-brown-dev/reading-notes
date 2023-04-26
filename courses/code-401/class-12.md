# Code 401 Reading 12

## Web Sockets

### What is a Web Socket?

- web socket is a communications protocol
- full duplex over TCP/IP
- real time data transfer from server
- different than HTTP because HTTP is not full duplex (send and receive continuously, at the same time)

### Describe the Web Socket request/response handshake and what happens once the connection is established

- client sends handshake request (HTTP request)
- server accepts and establishes connection, no longer HTTP
- "3 way handshake"
  - client request goes to server
  - server establishes connection with client
  - client confirms established connection to server

### Web Sockets provide a standardized way for the server to send content to a client without first receiving a ____ from that client

request

## Socket.io Tutorial

### What does the event handler io.on() do?

this handler turns the socket event handler one (it can open and close sockets for client traffic)

### Describe some possible proof of life or proof that the code works as expected

- run a terminal window with a client and server, try to connect to the server with the client, see what happens
- saw this demonstrated without an express server, if tried myself or used docs, would have started an express app

### What does socket.emit() do?

- socket.emit allows custom events to be created and fired
- socket.io has additional functionality that is not part of WebSocket spec

## Socket.io vs Web Sockets

### What is the difference between WebSocket and Socket.IO? (think Git and GitHub, or OAuth and Auth0)

- Socket.io is a library/implementation of WebSocket, which is a standardized protocol
- Socket.io incorporates additional features that are not part of the spec, but that are commonly added with separate libraries when spec-only implementations are used

### When would you use Socket.IO?

- when you want a fully featured implementation of websocket
- when you don't want to add the features of socket.io separately

### When would you use WebSockets?

- if your project must be compatible with systems that can't use socket.io

## Videos

### OSI Model Explained

### What are a couple of key takeaways from this video?

- OSI standardizes protocols for network intercompatibility across architectures
- Application layer for all user level apps that use the internet to communicate
- Presentation layer translates data to binary (data compression, lossy/lossless) decryption
- Session layer for authentication/authorization
- Transport layer for flow control, error control (adds checksum) TCP, UDP
- Network layer, packets, logical addressing, routing
- data link layer - sends and receives IP packets - CSMA - controls data transmission - error control
- physical layer - copper/fiber - information is actually sent as electrons over this layer

### TCP Handshakes Explained

### Translate the gist of this video to a non-technical friend

TCP handshake goes like this:

1. client (you) sends sync request (SYN) to server, with a sequence number and a SYN number
2. server responds with sync acknowledgement (SYN-ACK), with sequence number incremented by 1, as "ACK Number", and same SYN number
3. client sends acknowledgement (ACK), with SYN number reset to 0

[Go back home](/../reading-notes/)
