FROM node:current-alpine

WORKDIR /app

ENV PATH /app/node_modules/.bin:$PATH

COPY package.json ./
COPY package-lock.json ./

RUN npm install nodemon

COPY . ./

EXPOSE 3001

CMD [ "npm", "start" ]