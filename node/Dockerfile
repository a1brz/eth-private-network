FROM ethereum/client-go:v1.8.19

COPY data /root/.ethereum
COPY genesis.json .
COPY password .
RUN geth init genesis.json

EXPOSE 8545
EXPOSE 30303