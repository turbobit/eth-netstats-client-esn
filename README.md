ESN Network Intelligence API
============
[![Build Status][travis-image]][travis-url] [![dependency status][dep-image]][dep-url]

## forked from https://github.com/OpenCommunityCoin/eth-netstats-client-api

This is the backend service which runs along with ethereum and tracks the network status, fetches information through JSON-RPC and connects through WebSockets to [eth-netstats](https://github.com/turbobit/eth-netstats) to feed information. For full install instructions please read the [wiki](https://github.com/ethereum/wiki/wiki/Network-Status).

Live Work : https://escstats.gonsmine.com


## Prerequisite
* ESN node ( https://github.com/ethersocial/go-esn )
* npm


## Configuration

edit .env file

```
DE_ENV=production
RPC_HOST=localhost
RPC_PORT=9545
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


[travis-image]: https://travis-ci.org/turbobit/eth-net-intelligence-api.svg
[travis-url]: https://travis-ci.org/turbobit/eth-net-intelligence-api
[dep-image]: https://david-dm.org/turbobit/eth-net-intelligence-api.svg
[dep-url]: https://david-dm.org/turbobit/eth-net-intelligence-api
