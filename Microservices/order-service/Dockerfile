FROM node:20-alpine

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install --omit=dev

COPY . .

# Order Service runs on Port 3002
ENV PORT=3002
EXPOSE 3002

CMD ["node", "app.js"]