FROM ethereum/client-go:alltools-v1.8.20

COPY keystore /root/.ethereum/keystore
COPY genesis.json .
COPY password.txt .
RUN geth init genesis.json

# geth
EXPOSE 8545
EXPOSE 30303

# bootnode
EXPOSE 30301/udp

# swarm
EXPOSE 8500
EXPOSE 30399