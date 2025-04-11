FROM node:latest AS builder

WORKDIR /app

COPY package.json .

RUN npm install

FROM node:hydrogen-alpine AS final 

WORKDIR /app

COPY --from=builder /app .

COPY .env .   

EXPOSE 5000

CMD ["npm","start"]
