# Use Node 20 Alpine (small image)
FROM node:20-alpine

# Set working directory inside container
WORKDIR /app

# Copy package.json first (for efficient caching)
COPY package*.json ./

# Install dependencies
RUN npm install --production

# Copy rest of the app files
COPY . .

# Expose port
EXPOSE 3000

# Command to run app
CMD ["node", "index.js"]
