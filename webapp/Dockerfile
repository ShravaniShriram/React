FROM node:18

# Set the working directory inside the container
WORKDIR /app

# Copy only the package.json and package-lock.json first
COPY package*.json ./

# Install dependencies
RUN npm install --legacy-peer-deps

# Copy the rest of the app files
COPY . .

CMD ["npm" , "start"]
