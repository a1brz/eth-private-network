FROM node:8-alpine

RUN apk add --no-cache git make python g++
RUN git clone https://github.com/ethnamed/eth-explorer.git

WORKDIR /eth-explorer
RUN npm install -g bower && npm install && bower install --allow-root
CMD sed -i "s/209.126.79.177/$GETH_NODE_IP/" app/config.json && npm start

EXPOSE 8000