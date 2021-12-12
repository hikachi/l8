FROM node:alpine
ENV NODE_OPTIONS=--openssl-legacy-provider
WORKDIR '/app'
COPY package.json .
RUN npm install
USER node
COPY --chown=node:node . /app
CMD ["npm", "run","start"]
