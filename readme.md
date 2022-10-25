# Node starter

## Introduction

This is a server made with nodejs, express and typescript. It uses deployment tools such as docker and pm2.

## Instructions

- `npm install` or `yarn`
- Run locally by renaming env.template to env.test.local .

## Available Commands for the Server

- Run the Server in production mode : `npm run start` .
- Run the Server in development mode : `npm run dev` .
- Run all unit-tests : `npm test` .
- Check for linting errors : `npm run lint` .
- Fix for linting : `npm run lint:fix` .

### Docker :: Container Platform

[Docker](https://docs.docker.com/get-docker/) Install.

- starts the containers in the background and leaves them running : `docker-compose up -d`
- Stops containers and removes containers, networks, volumes, and images : `docker-compose down`

Modify `docker-compose.yml` and `Dockerfile` file to your source code.

### PM2 :: Advanced, Production process manager for Node.js

[PM2](https://pm2.keymetrics.io/) is a daemon process manager that will help you manage and keep your application online 24/7.

- production mode :: `npm run deploy:prod` or `pm2 start ecosystem.config.js --only prod`
- development mode :: `npm run deploy:dev` or `pm2 start ecosystem.config.js --only dev`

Modify `ecosystem.config.js` file to your source code.

### Swagger :: API Document

To visualize Swagger in development mode at visit `http://localhost:3000/api-docs` .

### Postman :: API Document

There is an included file called Node-starter.postman_collection.json with the postman project.

## 💳 License

[MIT](LICENSE)
