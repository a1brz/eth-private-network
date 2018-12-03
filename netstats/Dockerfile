FROM node:8-alpine

RUN apk add --update git
RUN npm install -g grunt
RUN git clone https://github.com/cubedro/eth-netstats.git

WORKDIR /eth-netstats
RUN npm install && grunt
CMD WS_SECRET=$WS_SECRET npm start

EXPOSE 3000