FROM node:16-buster
WORKDIR /app
COPY package*.json ./
RUN ls -la /app
RUN npm ci --only=production
COPY . .
EXPOSE 3000
CMD ["npm", "start"]