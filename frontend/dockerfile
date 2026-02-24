# Stage 1 - Build Angular
FROM node:18 AS build

WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .
RUN npm run build

# Stage 2 - Nginx
FROM nginx:alpine

# REMOVE default nginx files
RUN rm -rf /usr/share/nginx/html/*

# COPY Angular build output
COPY --from=build /app/dist/angular-15-crud/ /usr/share/nginx/html/