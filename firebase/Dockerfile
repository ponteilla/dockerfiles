FROM node:lts-alpine

ENV FIREBASE_VERSION=8.1.1

RUN npm install -g firebase-tools@${FIREBASE_VERSION}

ENTRYPOINT ["firebase"]
