# Use a lightweight Node.js image as a base
FROM node:18-alpine
# Copy package.json and install dependencies
COPY package.json ./
RUN npm install
# Copy the rest of the application code
COPY . .
# Expose the port your app runs on (e.g., 3000 for Node, 8000 for Python/Django/Flask)
EXPOSE 3000
# Command to run the application
CMD ["node", "server.js"]