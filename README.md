# AWS Websocket Messaging

> This repo contains Serverless Framework project for a simple AWS Websocket chat app

### Setup

> Install required npm packages first

```shell
$ npm install
```

> Install Serverless Framework globally

```shell
$ npm install -g serverless
```

> Install required Python packages

```shell
$ pip install -r python-packages.txt -t ./lib/python
```

> Deploy into AWS

```shell
$ serverless deploy --stage dev
```
> Creating a Coturn server
```
Create a EC2 instance with ALL_UDP ports open to the internet
sudo -i
apt-get update && apt-get install libssl-dev libevent-dev libhiredis-dev make -y 
apt install coturn
turnserver -a -o -v -n -u username:password -p 3478 -L private -r someRealm -X public/private --no-dtls --no-tls
```

> Connecting to Front-end.
```
WebRTCChat.html Change values of
Endpoint of websockets api 
IP address (public)
Port value (3478).
Username 
Password 
In S3 bucket host Html page
Enable public 
```

