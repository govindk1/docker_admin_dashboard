#  Dockerfile for Node Express Backend

FROM node:12.2.0-alpine
# Create App Directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

#COPY package.json and lock.json to container
COPY ./package*.json ./

# Install Dependencies
RUN npm install --silent

# Copy app source code
COPY . .

# Exports
EXPOSE 3000

CMD ["npm","start"]
