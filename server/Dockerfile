# Use a named build stage for production
FROM node:14 AS Production

ENV NODE_ENV=production

WORKDIR /server

# Copy the package.json and yarn.lock files to the container
COPY package.json yarn.lock ./

# Install dependencies using yarn
RUN yarn

# Copy the rest of the application code to the container
COPY . .

# Rebuild bcrypt inside the container
RUN npm rebuild bcrypt --build-from-source

# Specify the command to start the application
CMD ["yarn", "start"]
