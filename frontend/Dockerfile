#Use Node.js 16 as the base image
FROM node:16

# Set the working directory
WORKDIR /app

# Copy the package.json and package-lock.json files to the working directory
COPY package*.json ./

# Install the dependencies
RUN npm install

# Copy the rest of the project files to the working directory
COPY . .

# Expose port 8000
EXPOSE 8000

#Specify the command to run the application
CMD [ "npm", "start" ]