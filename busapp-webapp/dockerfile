# Using Node.js 16 as the base image
FROM node:16

# Setting up the working directory
WORKDIR /app

# Copying package.json and package-lock.json to the container
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the application code
COPY . .

# Build the React app (if applicable)
RUN npm run build

# Expose port 3000 for the app
EXPOSE 3000

# Start the server
CMD ["node", "serve.js"]
