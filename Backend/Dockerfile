# Use Node.js as base image
FROM node:18-alpine AS builder

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package.json package-lock.json ./

# Install dependencies
RUN npm install --production

# Copy application files
COPY . .

# Expose backend port
EXPOSE 5000

# Start the backend server
CMD ["node", "server.js"]
