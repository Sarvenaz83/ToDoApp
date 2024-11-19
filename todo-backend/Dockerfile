# Använd en officiell Node.js-bild
FROM node:18

# Sätt arbetskatalogen i containern
WORKDIR /usr/src/app

# Kopiera package.json och installera beroenden
COPY package*.json ./
RUN npm install

# Kopiera resten av applikationen
COPY . .

# Exponera porten
EXPOSE 5000

# Starta applikationen
CMD ["node", "server.js"]
