# Ethereum PoA private network
A Docker based implementation of blockchain network for testing and development purposes including:
- 1 Bootnode
- 1 Ethereum node
- 2 Ethereum miner nodes
- 2 [Swarm](https://swarm-gateways.net/bzz:/theswarm.eth) nodes (distributed storage platform)
- [Ethereum Network Status Dashboard](https://github.com/goerli/ethstats-server)

Using Proof-of-Authority consensus instead of Proof-of-Work.
New block creates every 5 seconds.

## Prerequisites
You should have installed Docker and Docker Compose in your machine.

## Run
```bash
git clone https://github.com/a1brz/eth-private-network.git
cd eth-private-network
docker-compose up
```

After all you can find:
- Ethereum Network Stats at [http://localhost:3000](http://localhost:3000)
- Node 1 RPC access at [http://localhost:8545](http://localhost:8545)
- Node 2 (miner) RPC access at [http://localhost:8546](http://localhost:8546)
- Node 3 (miner) RPC access at [http://localhost:8547](http://localhost:8547)
- Swarm Node 1 HTTP access at [http://localhost:8500](http://localhost:8500)
- Swarm Node 2 HTTP access at [http://localhost:8501](http://localhost:8501)
