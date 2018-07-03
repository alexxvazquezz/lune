FROM node:8

RUN apt-get install -y git

WORKDIR /app

COPY ../user-portal /app

EXPOSE 8080

RUN npm install http-server -g

RUN npm install && npm run build

CMD http-server ./dist