# Define the base image. Node is the runtime environment for JavaScript.
FROM node:14

# Set the working directory in the container to /app
WORKDIR /app

# Copy package.json and package-lock.json into the directory /app in the container
COPY package*.json ./

# Install the dependencies in the container
RUN npm install

# Copy the rest of the code into the container
COPY . .

# Expose port 3000 to be able to access it from the outside
EXPOSE 3000

# The command to run the app
CMD [ "node", "app.js" ]