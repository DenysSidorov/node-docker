# install image for docker
FROM node:8

# Set app directory in container like work-directory
WORKDIR /usr/src/app

# Copy package.json file to WORKDIR for installing app dependencies
COPY package*.json ./

# Install all dependencies from package.json
RUN npm install


# Copy app source code where we have dockerfile to WORKDIR
COPY . .

#Expose port for particular docker-container
EXPOSE 8082

# RUN these commands in docker-container
CMD [ "npm", "start" ]
