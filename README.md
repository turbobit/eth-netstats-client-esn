ESN Network Intelligence API
============
[![Build Status][travis-image]][travis-url] [![dependency status][dep-image]][dep-url]

This is the backend service which runs along with ethereum and tracks the network status, fetches information through JSON-RPC and connects through WebSockets to [eth-netstats](https://github.com/cubedro/eth-netstats) to feed information. For full install instructions please read the [wiki](https://github.com/ethereum/wiki/wiki/Network-Status).

Live Work : https://escstats.gonsmine.com


## Prerequisite
* ESN node ( https://github.com/ethersocial/go-esn )
* npm


## Configuration

edit .env file

```
DE_ENV=production
RPC_HOST=localhost
RPC_PORT=8545
API_HOST=localhost
API_PORT=8080
API_URL=/api/stats
LISTENING_PORT=50505
INSTANCE_NAME=<your name>
CONTACT_DETAILS=<contac detail>
WS_SERVER=wss://escstats.gonsmine.com
WS_SECRET=EtherSocial
VERBOSITY=2
```

## Run

Run it using node:

```bash
node app.js
```



It will stop the current netstats client processes, automatically detect your ethereum implementation and version, update it to the latest develop build, update netstats client and reload the processes.
