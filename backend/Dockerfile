# 1. Base image
FROM node:18

# 2. Set working directory
WORKDIR /app

# 3. Install dependencies
COPY package*.json ./
RUN npm install

# 4. Copy all code
COPY . .

# 5. Expose port (Express server)
EXPOSE 5000

# 6. Start app
CMD ["npm", "start"]