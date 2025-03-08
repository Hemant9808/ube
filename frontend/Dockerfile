# Use Node.js as base image
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package.json and install dependencies
COPY package.json package-lock.json ./
RUN npm install

# Copy all frontend files   
COPY . .

# Expose frontend port
EXPOSE 5173

# Start the frontend development server
# CMD ["npm", "run", "dev"]
CMD ["npm", "run", "dev", "--", "--host"]

