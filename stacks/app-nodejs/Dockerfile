# Use an official Node.js runtime as a parent image
FROM node:24

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy the package.json and install dependencies
COPY package*.json ./
COPY dist/ ./

# Install dependencies
RUN npm install

# Expose port 3000 to the host
EXPOSE 3000

# Command to run the app
CMD ["node", "server.js"]
