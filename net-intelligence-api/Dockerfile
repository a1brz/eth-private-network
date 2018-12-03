FROM node:8-alpine

RUN apk add --update git
RUN npm install -g pm2
RUN git clone https://github.com/cubedro/eth-net-intelligence-api.git

WORKDIR /eth-net-intelligence-api
COPY app.json .
RUN npm install
CMD pm2 start app.json --no-daemon