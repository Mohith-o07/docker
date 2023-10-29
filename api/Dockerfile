FROM node:20-alpine

RUN npm i -g nodemon

WORKDIR /app   
#/app becomes root from this cmd onwards..
COPY package.json .

RUN npm i
#at build-time

COPY . .

EXPOSE 4000
# required for docker desktop port mapping

CMD ["npm", "run","dev"]
#at run-time