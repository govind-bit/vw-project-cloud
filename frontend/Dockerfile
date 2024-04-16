# Stage-1 & specify a name 'builder'
FROM  node:20-alpine3.17

# Create a directory  and go to the directory 
WORKDIR /usr/src/app

# Copy the package.json file to my current directory to install the necessary dependence  
COPY package.json .

# Install the dependence
RUN npm install

# Copy other files to my current directory
COPY . .

EXPOSE 5173

# Run nginx in the foreground
CMD ["npm", "run", "dev"]