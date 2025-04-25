# Utiliser l'image officielle Node.js
FROM node:18

# Définir le répertoire de travail dans le container
WORKDIR /home/node/app

# Copier package.json et package-lock.json pour installer les dépendances
COPY ./package*.json ./

# Installer les dépendances de l'application
RUN npm install

# Copier tout le reste du code dans le container
COPY ./ /home/node/app

# Exposer le port 3000
EXPOSE 3000

# Lancer l'application React
CMD ["npm", "start"]