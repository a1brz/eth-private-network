FROM node:8-alpine

RUN apk add --no-cache git make python g++ yarn
RUN git clone https://github.com/etherparty/explorer.git

WORKDIR /explorer
RUN sed -i "s/localhost/0.0.0.0/" package.json && \
    sed -i 's/"prestart": "npm install",//g' package.json && \
    sed -i 's/"postinstall": "bower install",//g' package.json

RUN yarn && yarn global add bower && bower install --allow-root

CMD sed -i "s/localhost/$GETH_IRC_IP/" app/app.js && yarn start

EXPOSE 8000