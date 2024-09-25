


FROM node:18-alpine

# Set the working directory
WORKDIR /app-frontend

# Copy the contents of the frontend application to the container
COPY . .

# Install Angular CLI globally with the compatible Node.js version
RUN npm install -g @angular/cli

# Install the project dependencies
RUN npm install --legacy-peer-deps

# Expose the port the app will run on
EXPOSE 4200

# Command to start the Angular application
CMD ["ng", "serve", "--host", "0.0.0.0"]
