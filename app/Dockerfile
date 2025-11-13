FROM node:18-alpine
WORKDIR /app
COPY ./src ./src
COPY ./spec ./spec
COPY package.json ./
COPY ./yarn.lock ./yarn.lock
RUN yarn install --production
CMD ["node", "src/index.js"]