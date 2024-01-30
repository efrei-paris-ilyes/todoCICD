# Utilisez une image Node.js comme base
FROM node:14

# Définissez le répertoire de travail dans le conteneur
WORKDIR /usr/src/app

# Copiez le fichier package.json et le fichier package-lock.json dans le conteneur
COPY package*.json ./

# Installez les dépendances
RUN npm install

# Copiez le reste du code source du client dans le conteneur
COPY . .

# Exposez le port 8080 utilisé par le client
EXPOSE 8080

# Commande pour démarrer le client
CMD ["npm", "run", "start"]
