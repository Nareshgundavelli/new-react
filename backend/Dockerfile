# Use Node.js base image
FROM node:20-alpine

# Set working directory
WORKDIR /app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install

# Copy source code
COPY . .

# Expose backend port (example: 5000)
EXPOSE 5000

# Start backend server
CMD ["npm", "start"]
