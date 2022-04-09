# syntax=docker/dockerfile:1
FROM node:12.18.1
LABEL org.opencontainers.image.source https://github.com/mariekiecoetzee/ghtraining-publish-package
WORKDIR /
COPY ["package.json", "./"]
RUN npm install --production
COPY . .
CMD [ "node", "index.js" ]