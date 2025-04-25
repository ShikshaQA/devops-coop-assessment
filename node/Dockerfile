# Use an official Node.js image
FROM node:18-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy only package files first to install deps
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application
COPY . .

# Start the app (change this if your entry point isn't index.js)
CMD ["node", "index.js"]

# Expose the port the app runs on
EXPOSE 3000
