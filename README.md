
***Video Conference Platform (VCP)***

**Description**

This application is a client-server application. The client-server connection is done with UDP, because this is for live conferences, so a liitle bit loss of packages over the internet won't cause big issues.
The client and the server use 2 ports 5000 and 6000. The 5000 is the main port: server listens to it, clients send their video packages with port 5000, and the 6000 is the secondary port: the clients listen to 6000 port to get the conference participants' video capture packages from the server.

**Dependencies**

In this project Open CV library is used for camera capturing.
Open CV version:4.10.0

**GUI**

The client has a GUI written with Swing libraries.

**The Problem**

Unfortunately, how much I googled, asked to AI(CHatGPT, Claude.ai), did some research, I couldn't find the right way to send images in bytes with udp and decode them. So, now I'm getting null WHen I try to decode the image, that's why participant's video is white.
