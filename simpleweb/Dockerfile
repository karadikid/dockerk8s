# Base Image
FROM node:alpine

# Working Directory for files and context
WORKDIR /usr/app

# Copy base applicaton logic
COPY ./package.json ./
RUN npm install

# Copy content
COPY ./ ./

# Start default application
CMD ["npm", "start"]
