# Backend Dockerfile
FROM node:18-alpine

WORKDIR /app

# Copy package files
COPY package*.json ./

# Install dependencies
RUN npm ci --only=production

# Copy backend source code
COPY . .

# Expose backend port (usually 5000 or 3001)
EXPOSE 5006

# Start backend server
CMD ["node", "server.js"]