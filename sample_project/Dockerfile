# Use official Node.js image
FROM node:20-alpine

# Set working directory inside container
WORKDIR /app

# Copy package files first for caching
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy all project files
COPY . .

# Expose the default Vite dev server port
EXPOSE 5173

# Let Vite listen on all interfaces (so it's reachable externally)
ENV HOST=0.0.0.0

# Start the Vite dev server
CMD ["npm", "run", "dev"]
