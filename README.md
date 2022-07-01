# libp2p-webrtc-star-issue
This repository serves as an example for the signalling server issues when using @libp2p/webrtc-star

# Requirements
Node version required: 16

You will also need an up and running libp2p signalling server.

If you did not install it yet, you can retrieve it using the following command: 

`npm i -g @libp2p/webrtc-star-signalling-server`

# Startup

In your terminal, use the following commands to start the app:

```
git clone https://github.com/BaptisteHubert/libp2p-webrtc-star-issue.git;
cd libp2p-webrtc-star-issue;
npm i;
npm start;
```
The app will be running on the address: `http://localhost:3000/`

# Steps to reproduce issue

1. Start the signalling server by running this command: 

`webrtc-star --host=127.0.0.1 --port=8001`

2. After that, open a browser tab and access to the app ([http://localhost:3000/](http://localhost:3000/))

3. Repeat step 2 with another tab

4. Peers should have discovered and connected to each other

5. Stop the signalling server

6. Each browser tab should display that they have been disconnected
