# Native vs. Web

As described in [Idea](project/idea.html) the 2 Options to create the Frontend for our 3d Printer to upload the files are either create a native application or create a web interface.

We chose Option 2 because of multiple reasons.
1. A native application must be backwards compatible. So we can't make breaking changes at the communication level. Because the Website will be hosted on the PI with the other programs, it is part of a unit. This will also allow us to test the whole PI better.
2. We develop on multiple OS and we (may, if the 3d printer gets finished) print on different OS. With the decision to make a website we change the os compatibility problem to browser compatibility problem.

With the upcomming [wasm](https://en.wikipedia.org/wiki/WebAssembly) standard, we may be able to [slice](todo/todo) in the browser and send the sliced file instead of slicing on the PI.

If -in the future- we choose to build an native application, the application can connect to the same [WebSocket](design/websocket.html) the website is using.
