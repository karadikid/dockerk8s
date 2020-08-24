# Base Image
FROM node:alpine

# Working Directory context for App
WORKDIR '/usr/app'

# Npm install
COPY package.json .
RUN npm install

# Content copy
COPY . .

# Start app
CMD ["npm", "start"]

