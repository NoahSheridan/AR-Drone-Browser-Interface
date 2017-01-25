Getting started
======
Connect to your ar drone 2 via WLAN, then run node.server.js open up localhost:3001 and you're ready to go.

Use 'W, A, S, D' to move front, back and sideways. Use your 'I, K, J, L' to go up/down or turn clockwise/counter clockwise.
The  number keys '1-5' can be used to do flips in the direction of the key.
'SPACE' for taking off and 'esc' for landing.

When you crash use 'e' to recover from emergency mode.

This project is heavily inspired from https://github.com/functino/drone-browser .
I edited the HTML and CSS code to change the screen layout and edited the javascript to use different keys for operations.

Dependencies
=======
You can install/update the node dependencies via `npm install -d`.
Dependencies for client code are managed via bower ( https://github.com/twitter/bower ). 
You need to have `ffmpeg` installed (it's used for the picture stuff)

TODO
======
- use getUserMedia/the webcam to control the drone (like magic xylophone...)
- add a slider to make the speed/duration of actions configurable
- toggle between takeoff/land buttons or disable takeoff button after takeoff...
- maybe change the "recover" button to send a land command first (because otherwise the drone tries to start again...)
- only show the recover button when the drone is in emergency mode
- use canvas to draw angle-stuff or rotate the picture stream accordingly
- get rid of the (sometimes) long lag of the picture stream 
- make it work without ffmpeg (skip the picture stuff then....)