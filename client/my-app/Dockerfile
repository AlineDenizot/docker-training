FROM node:alpine

WORKDIR /app
ENV PATH /app/node_modules/.bin:$PATH
COPY package*.json ./
COPY yarn.lock ./
RUN yarn install
COPY src src
COPY public public

CMD ["yarn", "run", "start"]