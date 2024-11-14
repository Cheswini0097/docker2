# Use a lightweight Node.js image based on Alpine Linux
FROM node:20

# Set the working directory for the application
WORKDIR /opt/server

# Copy package.json and other necessary files
COPY package*.json .
COPY index.js .

# Install dependencies
RUN npm install

# Expose the port the app will listen on
EXPOSE 8080

# Set the database host environment variable
ENV DB_HOST="mysqlcont"

# Start the app
CMD ["node", "index.js"]