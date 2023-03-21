# web-stream
A NodeJS &amp; React based web app, creating a live stream from a device's camera to a web page.

About
Using Socket.io, to create Peer to Peer communications. This enables us to share real time media streaming between client server.
Socket.io utilises the 'WebSocket protocol' - providing communications over a TCP connection.
On connecting to a 'socket' when the server receives a message it then displays it automatically to all connected clients. Therefore, using this functionality we can create a single live stream, that can be watched by supposedly thousands of connected clients (based on what some people have tested).

To run:
 - To run locally from this directory:
    - 'cd backend' && npm start
    - 'cd frontend' && npm start
    - go to localhost:3000/
    - to watch a current live stream: go to localhost:3000/watch
    - to broadcast: go to localhost:3000/broadcast

- I also deployed a Heroku app in order to view it live:
    - go to https://web-stream-frontend.herokuapp.com/

What I would look into in the future:
    - WebRTC to replace Socket.io or work along side it.
    - Additional broadcasting rooms and allow people to watch different streamers.
    - Security & automated testing. Currently broadcasts can just be overruled by the next person to go to the broadcast url, this could be fixed by providing unique broadcasting urls for broadcasters. Or simply allow only one broadcaster at a time. I have Jest setup in order to start testing, I would add to this and set up various unit tests. Checks for stream start and end etc.
    - TypeScript, for bug solving and readability.
    - Redux, for better state control throughout the site rather than by components.
    - Styling, of course make it all look nicer, provide root css styles for use throughout the website. Favicon for the website tabs. Full screen stream etc.
    - Link to GoDaddy url.

