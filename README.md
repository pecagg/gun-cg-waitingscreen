# gun-cg-waitingscreen
Waiting screen for Road to Rio made with gun.js, a fork from https://github.com/filiphanes/gun-overlays
Simple and powerfull remote controlled html pages useful for overlays in OBS Studio, Casper CD, XSplit or simply fullscreen browser.

## Features
- server holds overlay state
- on refresh or reconnect, state is updated from server for overlay and controller so you don't loose texts etc.
- multiple overlay-controller groups on 1 server instance (via different websocket paths)
- server is needed only for first connect, both controller and overlay holds state info

# Install
NodeJS is needed. You can download it from https://nodejs.org/en/

    npm install

# Run
## 1. Run websocket server
Node server:

    node server.js

## 2. Open controller
Open in browser `roadtorio/kontrola.html`.

## 3. Open overlay
Open in browser `roadtorio/pregame.html`

## OBS Studio
1. Click the plus button under Sources
2. Select BrowserSource
3. Name the source and click "OK"
4. Check the "Local file" box
5. Click the "Browse" button on the right and select the client.html you want to use
6. Set the Resolution to 1920x1080 (Width: 1920; Height: 1080) or the overlay resolution
7. Set FPS to you stream FPS (examples: 25, 30, 50, 60)

## Caspar CG
https://github.com/CasparCG/help/wiki/Media:-HTML-Templates

## ProPresenter
ProPresenter browser capabilities in versions 6 and 7 are very limited, and this overlays are not usable.
https://learn.renewedvision.com/propresenter6/the-features-of-propresenter/web-view

## XSplit
https://www.xsplit.com/broadcaster/manual/sources/webpage

# New overlays
You can create your own overlay and associated controller without implementing server.

## Server API
https://gun.eco/docs/API

# Copyright
This project was made by 
https://raw.githubusercontent.com/filiphanes/gun-overlays/
I've just tweaked it for my own use
