# Use the official Node.js image as base
FROM node

# Set the working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application
COPY . .

# Expose port 3000 (or the port your Nest.js app is configured to use)
EXPOSE 3000

# Start the Nest.js application
CMD ["npm", "start"]
