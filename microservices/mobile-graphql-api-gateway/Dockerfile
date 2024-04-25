# Use the official Node.js 20.12.2 LTS image as the base image
# https://hub.docker.com/layers/library/node/lts-alpine3.19/images/sha256-e18f74fc454fddd8bf66f5c632dfc78a32d8c2737d1ba4e028ee60cfc6f95a9b?context=explore
FROM node:lts-alpine3.19

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install project dependencies
RUN npm install

# Copy the rest of the application source code to the container
COPY . .

# Expose the port your Nest.js application is listening on
EXPOSE 3000

# Command to start your Nest.js application
CMD [ "npm", "run", "start:prod" ]