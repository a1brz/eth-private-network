FROM node:8-alpine

RUN apk add --update git
RUN npm install -g grunt
RUN git clone https://github.com/goerli/ethstats-server.git

WORKDIR /ethstats-server
RUN sed -i "s/Testnet/Ethereum/" src/views/layout.jade
RUN npm install && grunt poa
CMD npm start

EXPOSE 3000