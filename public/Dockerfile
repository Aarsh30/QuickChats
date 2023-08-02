# Use a named build stage for production
FROM node:14 AS Production

# Set the NODE_ENV environment variable to "production" (Remove the spaces around the equal sign)
ENV NODE_ENV=production

# Set the working directory in the container
WORKDIR /public

# Copy the package.json and package-lock.json files to the container (Use package-lock.json for npm)
COPY package.json package-lock.json ./

# Install dependencies using npm (since package-lock.json is used)
RUN npm install

# Copy the rest of the application code to the container
COPY . .

# Install additional dependencies (if any) using yarn (Ensure you have a yarn.lock file)
RUN yarn

# Specify the command to start the application
CMD ["yarn", "start"]
