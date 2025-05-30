# backend/Dockerfile
FROM node:20-alpine

WORKDIR /app

RUN apk add --no-cache netcat-openbsd
COPY package*.json ./
RUN npm install

COPY . .

ENV PORT=8888
EXPOSE 8888

CMD ["sh", "-c", "npm run setup && npm start"]

