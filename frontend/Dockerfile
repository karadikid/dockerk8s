# Builder Phase
FROM node:alpine as builder
WORKDIR /app
COPY package.json .
RUN npm install
COPY . .
RUN npm run build

# Run Phase - FROM keyword signifies new Phase
FROM nginx
COPY --from=builder /app/build /usr/share/nginx/html


