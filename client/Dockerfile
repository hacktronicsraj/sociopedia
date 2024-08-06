FROM node:16-buster
WORKDIR /app
COPY package.json ./
COPY package-lock.json ./
RUN npm install
RUN npm ci --only=production
COPY . .
EXPOSE 3000
CMD ["npm", "start"]