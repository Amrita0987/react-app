# Pull Official Base Image
FROM node:latest

# Set Working Directory
WORKDIR /src

# Install App Dependencies
COPY ["package.json", "package-lock.json", "/src/"]
RUN yarn

# Add App
COPY [".", "/src"]

# Start App
CMD ["npm", "build"]
