FROM node:18

# Set working directory
WORKDIR /app

# Copy package files and install deps
COPY package*.json ./
RUN npm install

# Copy rest of the frontend
COPY . .

# Expose the React dev server port
EXPOSE 3000

# Start the app with host binding
CMD ["npm", "start"]
