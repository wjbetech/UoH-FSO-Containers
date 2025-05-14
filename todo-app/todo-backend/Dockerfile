FROM node:22-slim

WORKDIR /todo-backend

COPY package*.json ./

RUN npm ci

COPY . .

ENV DEBUG=todo-backend:*

USER node

CMD ["npm", "start"]