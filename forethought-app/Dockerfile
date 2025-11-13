# Use the official Node.js LTS image
FROM node:18-alpine

# Set working directory inside the container
WORKDIR /usr/src/app

# Copy package files first for dependency installation
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy all application source code
COPY . .

# Expose the application port
EXPOSE 8080

# Start the Node.js app (main file is index.js)
CMD ["node", "index.js"]
