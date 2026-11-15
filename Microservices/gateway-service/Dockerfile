FROM node:20-alpine

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install --omit=dev

COPY . .

# Gateway Service runs on Port 3003
ENV PORT=3003
EXPOSE 3003

CMD ["node", "app.js"]