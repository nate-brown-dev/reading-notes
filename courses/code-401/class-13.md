# Code 401 Reading 13

## Socket.io Chat Example

### Explain to a non-technical recruiter what the Chat Example (above) does

the chat example establishes a duplex connection (live 2 way) that allows users to send and receive messages in real time

### What proof of life are we getting on the backend from the above app?

the server is console logging received messages

### Socket.IO gives us the i0.emit() method to send an event to everyone. What flag would you use if you want to send a message to everyone except for a certain emitting socket?

socket.broadcast.emit is for emitting messages to everyone except the sender

## Rooms

### What is a room and how might a room be useful?

a room is a subdivision of the socket that allows traffic to only be sent and received by users in the room

### How do you join a room?

joining the room is an event emitted by the joining clients

socket.emit("join-room", data)

followed by the server receiving the "join-room" event, and responding with a join action

socket.on("join-room", data)
  socket.join("room name")

### how do you leave a room?

client send socket.emit("leave-room")

## Namespaces

### What is a Namespace and what does it allow you to do?

a namespace is a subdivision of the websocket connection that allows logic to be split over a shared connection

the namespace is more inclusive than a room

io > namespace > room

### Each namespace potentially has its own what? (hint: 3 things)

- event handlers
- rooms
- middlewares

### Discuss a possible use case for separate namespaces

an online store with multiple departments

- shipping
- customer service
- shopping cart
- product reviews
- employee communication
