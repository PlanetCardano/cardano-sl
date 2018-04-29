
### Run a Cardano settlement layer node
Run a very lean Cardano settlement node. This is an alternative to having to [do it yourself](https://github.com/input-output-hk/cardano-sl/blob/master/docs/how-to/build-cardano-sl-and-daedalus-from-source-code.md).

### Usage
```
docker pull planetcardano/cardano-sl
docker up -d
curl -sfk https://localhost:8090/api/settings/sync/progress | jq
```

## Requirements
This container requires the following paths to exist with write permissions
* /cardano/state-wallet-mainnet
* /cardano/state-wallet-mainnet-tls

## Usage
`docker-compose up --build -d`
