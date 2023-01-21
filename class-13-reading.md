# Class 13 reading

## Explain to a non-technical recruiter what the Chat Example (above) does

This example is us creating a basic chatroom app where if anyone posts any form of text then EVERYONE will see that text on their screen.

## What proof of life are we getting on the backend from the above app?

We are getting our `listening on 3000` and as well as constant updates of when the user is connected and when the user is disconnecting (upon each refresh in this example).

## Socket.IO gives us the i0.emit() method to send an event to everyone. What flag would you use if you want to send a message to everyone except for a certain emitting socket?

We would use the `broadcast` flag

`io.on('connection', (socket) => {
  socket.broadcast.emit('hi');
});`

## What is a room and how might a room be useful?

The concept of a room is essentially like a room of a house. One room is the Tv room, one room is the Office, and the other room is the kitchen, You or anyone can enter (and leave) any room that they would like (or whatever room they feel they see most fitting for their needs at the time). This (in the context of a an app) is we are able to have various rooms available that are based around different topics or interests, this makes it easy to take care of multiple clients and their interests.

## How do you join a room?

You would use the `on` method.

`io.on("connection", (socket) => {socket.join("some room");});`

Here you are using the `on` method to join a specific socket(room) which is being delcaired as an argument in the `join` method

then from there you would use `to` or `in` when broadcasting or emitting.

`io.to("some room").emit("some event");`

## how do you leave a room?

You can leave the rooms use the disconnecting event

`
io.on("connection", socket => {
  socket.on("disconnecting", () => {
    console.log(socket.rooms); // the Set contains at least the socket ID
  });

  socket.on("disconnect", () => {
    // socket.rooms.size === 0
  });
});
`

## What is a Namespace and what does it allow you to do?

Namespaces is a communication channel. This allows you to split the logic of your app over a share connection. This is also a called multiplexing.

## Each namespace potentially has its own what? (hint: 3 things)

- Event Handlers
- Rooms
- Middleware

## Discuss a possible use case for separate namespaces

IF you want to create a special namespace that only auth. users have access to. This would seperate the logic so that the logic required for the auth users is seperate from the rest of the application.

## What are your learning goals after reading and reviewing the class README?

It would be pretty interesting to understand what a message server requires to make it work. I would have not figured that the background is doing so much.

## Things I want to know more about

I honestly want to grasp what is going on with the sock.io deal. Its still something I dont (completely) understand.
