---
layout: single
sidebar:
  nav: "docs"
---

### Architecture
------------------

The One Game platform contains both a client side and a server side.

The client side is the interface that connects the real and the virtual world and consists of a game interface for game players, and developers’ tools for game developers. Initially, we will launch a desktop PC client, which will be followed by mobile client and VR client.

The server side is built on top of Deepbrain Chain (DBC), which is a low-cost, private, flexible, safe, and decentralized computing platform. The server side includes two parts: smart contracts on Deepbrain Chain, and mining services on Deepbrain Chain’s computing platform deployed by miners. Any user can become a miner by downloading One Game’s source code from an online repository, and uploading a compiled binary to Deepbrain Chain’s computing platform to execute. In this way, through Deepbrain Chain hosting, miners provide computing and storage resources to One Game, and are rewarded One Game Tokens (OGT) through simulated mining process.

All key judgment and logic are implemented on the server side. The gaming clients only conduct rendering and computations that don’t affect the game results or use rankings.


