FROM node:lts-alpine
RUN apk add --no-cache sqlite-libs
WORKDIR /hookd
CMD node src/index.js
COPY package.json package-lock.json ./
RUN npm install --omit=dev
COPY src src
