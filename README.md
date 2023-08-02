# Snappy - Chat Application 
Snappy is Peer to Peer Chat Application built using react js ,nodejs and using the holepunch which help to communicate the message and make it easy process to chat among each other. 



## Installation Guide

### Requirements
-

Both should be installed and make sure mongodb is running.

```shell
git clone
cd  directory
```
Now rename env files from .env.example to .env
```shell
cd public
mv .env.example .env
cd ..
cd server
mv .env.example .env
cd ..
```

Now install the dependencies
```shell
cd server
yarn
cd ..
cd public
yarn
```
We are almost done, Now just start the development server.

For Frontend.
```shell
cd public
yarn start
```
For Backend.

Open another terminal in folder, Also make sure mongodb is running in background.
```shell
cd server
yarn start
```

Done! Now open localhost:3000 in your browser.
