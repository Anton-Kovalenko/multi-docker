FROM node:alpine
WORKDIR /app
ENV PATH /app/node_modules/.bin:$PATH
COPY package*.json ./
RUN npm install
RUN npm install react-scripts -g
RUN apk --update add postgresql-client

COPY . ./
CMD ["npm", "run", "start"]