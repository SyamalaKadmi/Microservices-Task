#Use node.js image from DockerHub
FROM node:18-alpine

# Set the working directory
WORKDIR /app

# Copy package.json to handle dependencies installation
COPY package.json ./

# Install dependencies
RUN npm install

# Copy app.js
COPY app.js ./

# Expose the 3003 port for the gateway-service
EXPOSE 3003

# Start the node.js application
CMD ["node", "app.js"]
