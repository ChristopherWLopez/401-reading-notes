# Socket

## What is a Web Socket?

Websocket is a **communications protocol**( a system of rules that allows two or more entities of communications systems to transmit info via any variation of physical quantity... [taken from](https://en.wikipedia.org/wiki/Communication_protocol)) that provides **full duplex**(A full-duplex (FDX) system allows communication in both directions, and, unlike half-duplex, allows this to happen simultaneously[taken from](https://en.wikipedia.org/wiki/Duplex_(telecommunications)#FULL-DUPLEX)) communication over complex channels over a **TCP**(transmission control protocol.a connection-oriented communications protocol that facilitates the exchange of messages between computing devices in a network. It is the most common protocol in networks that use the Internet Protocol (IP); together they are sometimes referred to as TCP/IP. ) connection

## Describe the Web Socket request/response handshake and what happens once the connection is established

"The Websockey handshake uses the HTTP upgrade header to change fromt the HTTP protocol to the websocket protocol." [from wiki](https://en.wikipedia.org/wiki/WebSocket)

## Web Sockets provide a standardized way for the server to send content to a client without first receiving a ____ from that client

-request

This allows for ongoing communication (usually over port 443.... unless its port 80 which is unsecured)

Socket.io allowa real-time bi directional event based communication.

## What does the event handler io.on() do?

- The io.on event handler handles connection, disconnection, etc., events in it, using the socket object

## Describe some possible proof of life or proof that the code works as expected

We could utilize nodemon and write "hello world" within a made index file.

## What does socket.emit() do?

You are able to create custom events as well as "fire" them.

## What is the difference between WebSocket and Socket.IO? (think Git and GitHub, or OAuth and Auth0)

Web Socket is the protocol (like HTTP) (or language)

Socket.io us library that has all the functionality (the actions)

## When would you use Socket.IO?

When you would use multiple sockets at the same time. And when reliability and speed are of concern.

## When would you use WebSockets?

## What are a couple of key takeaways from this video?

I was blown away to see the layout and difference between these layers and all the layers are protocols

the OSI model was made to ensure connection between different software. These are like the set of rules.

## Translate the gist of this video to a non-technical friend

TCP is A effient and accurate form of communication. This is the communication that starts from the client side (syn) and the server responds with (syn-ack) and then the client responds with (ack) back to the server with the connnection. This feels like a secret handshake or password that is started. This is also like me knocking on the door with that 4 knock rythmn then you respond with that 2 rythmn then you unlock the door and then I open the door.

[info from](https://www.sdxcentral.com/resources/glossary/transmission-control-protocol-tcp/#:~:text=Transmission%20Control%20Protocol%20(TCP)%20%E2%80%93,referred%20to%20as%20TCP%2FIP.)
