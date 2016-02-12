# Socket IO client v1.45

Working with nodejs socket.io server v1.4.5.

## Use

Rename socket.io_working_reformatted.js to socket.io.js and replace the socket.io.js file in
the socket io client folder that you've already downloaded and included into your project.

## Disabled Compression

Line: 2076 of the re-formatted version
```
// disabled below check with 'false &&' to get around of a global.Buffer undefined error
   if (false && self.perMessageDeflate) {
```

## websocket Protocol Only

Have to use the websocket protocol, in conjunction with tiws or a similar websocket module:

eg.
io('https://server.ip:1234', { transports: ['websocket'] });



Will do a non re-formatted version, so it is easier to compare the differences.
