FROM node

ENV MONGO_DB_USERNAME=admin \
    MONGO_DB_PASSWORD=root

WORKDIR /app

COPY . .

RUN npm install

CMD ["node", "server.js"]