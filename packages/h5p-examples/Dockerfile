FROM node:lts

USER node
RUN mkdir /home/node/h5p-nodejs-library
WORKDIR /home/node/h5p-nodejs-library
COPY --chown=node:node . ./
RUN npm install

EXPOSE 8081
CMD [ "node", "build/examples/express.js" ]
