FROM node:hydrogen-alpine

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

COPY .env .

EXPOSE 5000

CMD ["npm","start"]

