FROM node:8-alpine

RUN apk add --update git
RUN npm install -g grunt
RUN git clone https://github.com/goerli/ethstats-server.git

WORKDIR /ethstats-server
RUN npm install && grunt poa
CMD WS_SECRET=$WS_SECRET npm start

EXPOSE 3000