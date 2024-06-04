#Use Node.js 16 as the base image
FROM node:16

# Set the working directory
WORKDIR /app

# Copy the package.json and package-lock.json files to the working directory
COPY package*.json ./

# Install the dependencies
RUN npm install

# Install nodemon globally
RUN npm install -g nodemon

# Copy the rest of the project files to the working directory
COPY . .

# Expose port 9000
EXPOSE 9000

#Specify the command to run the application
CMD [ "npm",  "start" ]