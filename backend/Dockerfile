# backend/Dockerfile
FROM node:18-alpine

WORKDIR /app

COPY package*.json ./
RUN npm install
RUN npm run setup

COPY . .

ENV PORT=8888
EXPOSE 8888

CMD ["npm", "start"]

