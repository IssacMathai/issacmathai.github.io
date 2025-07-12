---
title: "SwapBytes"
description: A Rust libp2p file bartering application for students to swap notes.
date: 2025-04-28 00:00:00 +0800
categories: [University]
tags: [Rust]
---

## Information
SwapBytes is a P2P file swapping application that is built using Rust and libp2p protocols. Users connect to a chatroom via mDNS or a rendezvous server and can then message, DM or initiate trades with each other. Interaction is handled through entering commands on the CLI. File swaps are reliant on both sides sending files, so one party cannot renege on their end of the deal. Additionally, file encryption and decryption have been implemented with the help of the Rust crypto_box crate. The code has been modularised into four rust files and is well documented with Rustdoc and comments.

The biggest challenge I faced was issues with multiple requests. For example, if Alice sent Bob two trade requests, Bob would only be able to accept the latest one. After a lot of time debugging with print statements, I finally discovered that the issue was related to the request response channel closing, although I did not understand why a second trade offer would close this channel. After some research into what could cause a channel to close, I realised that it could be due to the channel simply timing out. I then read over the request response protocol's documentation and figured out how to change the channel timeout duration to 30s, which fixed the issue.

I developed this application for an assignment of my Decentralised Web Applications course and got an A+. If I were to do it over again, I would create a GUI or even just a beautified terminal user interface using the Ratatui library. This would make the application look more friendly and appealing.

## Features
- Chatroom messaging.
- Direct messaging.
- Safe swaps -- both parties must send files in order to receive what they requested.
- Asymmetric encryption using the XSalsa20 algorithm thanks to the Cryptobox rust crate.