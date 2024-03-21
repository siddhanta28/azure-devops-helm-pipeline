# base image
FROM node:latest As base

# set working directory
WORKDIR /app

# Copy Content
COPY * ./
#COPY .env.production ./
#COPY .env.staging ./
#COPY webpack/ ./webpack
#COPY dist ./dist
#COPY public ./public

# Install Dependencies
RUN npm install 

# EXPOSE port
EXPOSE 3007

ENV ENV_NAME=production

# Start Application
#CMD ["sh", "-c", "npm", "run", "start:server:${ENV_NAME}"]
#CMD ["npm", "run", "start:server"]
CMD ["npm", "start"]