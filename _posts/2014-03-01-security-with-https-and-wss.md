---
layout: documentation
title: Security with HTTPS and WSS
categories:
 - documentation
---

We recommend that you access the hosted app via the secure URL: 

[https://app.flowhub.io/](https://app.flowhub.io/)

Your login and projects in the browser's local storage will not follow you between http and https. You'll need to login again, and sync your projects via Github.

## Connecting from hosted app to local noflo

It can be tricky to set up a secure websocket server (wss:) locally. Discussion in the noflo repository: [#11](https://github.com/noflo/noflo-nodejs/pull/11). It might be easier to keep using [http://app.flowhub.io/](http://app.flowhub.io/) in this case.
