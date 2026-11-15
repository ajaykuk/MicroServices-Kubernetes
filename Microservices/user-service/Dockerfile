FROM node:20-alpine

WORKDIR /usr/src/app

# Copy package.json (and package-lock.json if present)
COPY package*.json ./

# Install dependencies
RUN npm install --omit=dev

# Copy application source code (app.js)
COPY . .

# User Service runs on Port 3000
ENV PORT=3000
EXPOSE 3000

CMD ["node", "app.js"]