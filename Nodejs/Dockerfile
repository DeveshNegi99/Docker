# Using the official nodeJs image
FROM node:18

# Set the working Directory inside the container
WORKDIR /app

# Copy package.json first (better caching)
COPY package.json ./

# Install dependencies
RUN npm install

# Copy all other files to the image
COPY . .

# Set the environment variables
ENV NAME=world

# Expose the port
EXPOSE 3000

# Run the app
CMD ["node", "appfile.js"]
