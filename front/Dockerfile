#FRONT
FROM node:lts-alpine
RUN npm install -g http-server
RUN mkdir /app
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY npm run build
EXPOSE 5000
CMD ["http-server", "dist"]