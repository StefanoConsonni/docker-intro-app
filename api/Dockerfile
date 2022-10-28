FROM node:16-alpine

RUN npm install -g nodemon

# set the working directory
WORKDIR /app

# install dependencies
COPY package.json .
RUN npm install

# copy scripts to folder
COPY . .

# required for docker-desktop port mapping
EXPOSE 4000

# start the server
CMD ["npm", "run", "dev"]
