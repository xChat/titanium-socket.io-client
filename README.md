# Socket IO client v1.45

Tested with server v1.4.5 too.

## Use:

Rename socket.io_working_reformatted.js to socket.io.js and replace the socket.io.js file in
the socket io client folder you downloaded and included in your project.


Will do a not re-formatted version soon.


## Disabled compression

Line: 2076 of the re-formatted version
```
// disabled below check with 'false &&' to get around of a global.Buffer undefined error
   if (false && self.perMessageDeflate) {
```

## websocket protocol only

Have to use the websocket protocol, in conjunction with tiws or a similar websocket module:

eg.
io('https://server.ip:1234', { transports: ['websocket'] });

