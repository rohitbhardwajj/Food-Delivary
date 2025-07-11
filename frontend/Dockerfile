# 1. Base image
FROM node:18

# 2. Set working directory
WORKDIR /app

# 3. Copy package.json and install deps
COPY package*.json ./
RUN npm install

# 4. Copy all files
COPY . .

# 5. Expose port (Vite default port)
EXPOSE 5173

# 6. Start dev server
CMD ["npm", "run", "dev"]