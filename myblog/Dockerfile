FROM node:17-alpine

WORKDIR /app

COPY package.json .
COPY yarn.lock .

# Install dependencies
RUN yarn install

COPY . .

EXPOSE 5173

# Set the command to start the application
CMD [ "yarn", "dev" ]