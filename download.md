---
title: Download
excerpt: "Search for a page or post you're looking for"
---

To download the latest version go [here](https://github.com/Andrea055/nodeMyAdmin/releases) and download the first .zip in release

# How to execute

Unzip the file in a folder, then do

```bash
npm i
```

Now, create a file named .env where you need to write the encryption key for your db credentials(nodeMyAdmin don't save password without cryptography).

.env file should contain the following fields:

```dosini
KEY=""
IV=""
```

IV must be of 16 characters while key don't have any requrements.

Now to start nodeMyAdmin server run 

```bash
node server.js
```
By the way, I don't recommend this way but you can use PM2 to manage the server.
[More info here](https://github.com/Unitech/pm2).

Or if you don't want to use pm2, you can modify server.js(is an express server) to bind address or other things.
