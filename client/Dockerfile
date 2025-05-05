# Stage 1: Base build using Node
FROM node:18-alpine AS base

# Set working directory
WORKDIR /app

# Install dependencies
COPY package*.json ./
RUN npm install --production

# Copy full code
COPY . .

# Expose backend port
EXPOSE 5000

# Run the app
CMD ["npm", "start"]
