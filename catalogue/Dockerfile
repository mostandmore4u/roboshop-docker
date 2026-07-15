FROM node:20.20.2-alpine3.22
# creates /app and set the directory to /app
WORKDIR /app
COPY package.json .
COPY *.js .
RUN npm install
# in docker container names used as DNS
ENV MONGO_URL="mongodb://mongodb:27017/catalogue" \
    MONGO="true"
# image to container CMD instuction
CMD ["node","server.js"]
