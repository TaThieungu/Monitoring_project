## build stage ##
FROM node:18.18-alpine as build

WORKDIR /app
COPY . .

RUN npm install --force
RUN npm run build 

## run stage ##
FROM eclipse-temurin:17-jdk-alpine

COPY --from=build /app/dist/angular-ecommerce /usr/share/nginx/html

EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]