FROM node:20-alpine

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install --omit=dev

COPY . .

# Product Service runs on Port 3001
ENV PORT=3001
EXPOSE 3001

CMD ["node", "app.js"]