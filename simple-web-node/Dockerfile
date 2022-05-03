# Specify a base Image
FROM node:alpine

# To fix issue in newer node version
WORKDIR /usr/app

# Adding 2 COPY commands so that package isn't downloaded again using npm install
# because package hardly changes. This will help build this stage from cache 

# Locate and copy package.json
COPY ./package.json ./

# Install npm dependencies
RUN npm install

# Copy rest of the stuff, files which change usuall like index.js
COPY ./ ./

# Default command
CMD ["npm", "start"]

