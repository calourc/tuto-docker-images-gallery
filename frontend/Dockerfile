FROM node:16.15-alpine

WORKDIR /app

EXPOSE 3000

COPY package.json package-lock.json ./

RUN npm install --silent

RUN npm update chokidar

COPY . ./

CMD ["npm", "start"]
