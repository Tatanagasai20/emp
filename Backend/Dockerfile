FROM node:18-alpine

WORKDIR /app

# Copy package.json and install only production dependencies
COPY package*.json ./
RUN npm install --only=production --silent

# Copy source code
COPY . .

# Expose API port (change if different)
EXPOSE 5000

# Start the Node.js app
CMD ["npm", "start"]

