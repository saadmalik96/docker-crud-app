# Use Node.js LTS version as base image
FROM node:18

# Set working directory in container
WORKDIR /app

# Copy package.json and package-lock.json
COPY package.json package-lock.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application
COPY . .

# Expose the port the backend runs on
EXPOSE 8800

# Start the backend
CMD ["npm", "start"]
