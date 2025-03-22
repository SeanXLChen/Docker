# Base image
FROM node:23-alpine

# copy package.json to the container's folder
COPY package.json /app/

# copy the src folder to the container's folder
COPY src /app/src/

# go to the app folder
WORKDIR /app

# Execute commands
RUN npm install

# Expose the port your app runs on
EXPOSE 3000

# Start the application
CMD ["node", "src/server.js"]