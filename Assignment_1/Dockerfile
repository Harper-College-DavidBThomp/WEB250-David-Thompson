# References:
#   https://code.visualstudio.com/docs/containers/quickstart-node
#   https://docs.docker.com/develop/develop-images/dockerfile_best-practices/
#   Code From: https://en.wikiversity.org/wiki/Docker/Express

# Purpose: 
#   Installs express over port 3000, expecting file app.js
#   Docker Testing Instructions: 
#   docker build -t express-server .
#   docker run -d -p 3000:3000 --name=express-server express-server

FROM node:alpine
WORKDIR /usr/src/app

RUN npm install express
COPY . .

EXPOSE 3000
CMD ["node", "app.js"]
