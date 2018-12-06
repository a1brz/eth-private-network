FROM ethereum/client-go:alltools-v1.8.19

COPY keystore /root/.ethereum/keystore
COPY genesis.json .
COPY password.txt .
RUN geth init genesis.json

EXPOSE 8545
EXPOSE 8500
EXPOSE 30303
EXPOSE 30399