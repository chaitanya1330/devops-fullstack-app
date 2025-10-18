# Use Node.js 14.17
FROM node:14.17

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the frontend code
COPY . .

# Expose frontend port
EXPOSE 3000

# Start the frontend
CMD ["npm", "start"]

