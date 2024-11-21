# Simple-Distributed-Chat-Application
1. Introduction
1.1 Purpose:
This project aims to build a real-time, multi-user
chat application that enables multiple users to send
and receive messages in a distributed network. It
uses message passing to simulate communication
between nodes, ensuring that messages sent by one
user are visible to all other connected users.
1.2 Technologies Used:
 Frontend:
o HTML, CSS, JavaScript (Socket.IO)
 Backend:
o Flask (Python-based web framework)
o Socket.IO for real-time communication
2.1 Real-Time Messaging:
 Users can send and receive messages instantly,
without page refreshes, using WebSockets via
Socket.IO.
2.2 Multiple User Support:
 Multiple users can join the same chat room, and all
messages sent by any user are visible to every
connected client.
2.3 Broadcasting of Messages:
 Messages are broadcasted from the server to all
connected users, ensuring that everyone in the chat
can see the same content in real-time.
2.4 Simple User Interface:
 The user interface is intuitive, allowing users to
send messages easily and view the entire chat
conversation.
3. Project Workflow
3.1 Client-Side:
 Users enter a nickname and join the chat.
 A message is sent via a text input box.
 The client automatically updates the chat
window with the incoming messages from
other users.
3.2 Server-Side:
 Flask handles HTTP requests, serving the
frontend (chat page).
 Socket.IO is used to establish WebSocket
connections for real-time messaging,
broadcasting messages to all clients.
4. How the Application Works
4.1 Client Side Flow:
1. Nickname Input: The user enters a nickname upon
launching the application.
2.Message Sending: Users type their message in a
text input box and click "Send" or press Enter to
send the message.
3.Message Receiving: The client listens for
incoming messages from the server and
automatically updates the chat window.
4.2 Server Side Flow:
1. Connection: When a client connects to the server,
Flask starts handling HTTP requests, while
Socket.IO handles real-time communication.
2.Message Broadcast: When a user sends a
message, the server broadcasts the message to all
connected clients.
3. Disconnection: If a user disconnects, the server
informs all other users that the user has left the
chat.
Challenges Faced
During the development of the application, the following challenges
were encountered:
 Real-Time Messaging: Ensuring that messages are broadcasted
to all users instantly, without delay.
 Concurrency Handling: Managing multiple users effectively
and ensuring that each message is displayed to all clients
without errors or performance issues.
Future Enhancements
Private Messaging:
Allow users to send private messages to specific individuals rather than
broadcasting messages to all users.
User Authentication:
Implement login functionality to authenticate users before allowing them to join
the chat, ensuring secure user management.
Chat Rooms:
Enable users to create and join different chat rooms for more organized
conversations.
Message History:
Implement functionality to store and retrieve message history so that users can
view past messages even after restarting the application
