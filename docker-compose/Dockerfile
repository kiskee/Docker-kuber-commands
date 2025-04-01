FROM node:18-alpine

# Establece el directorio de trabajo
WORKDIR /app


COPY package.json .
RUN npm install
COPY . .

CMD  ["npm", "start"]