FROM node:16.13.2-alpine

EXPOSE 3000
ENV HOST 0.0.0.0

WORKDIR /react_app

COPY package*.json .

RUN npm install

COPY . .

RUN npm run build

CMD ["npm", "run", "start"]
