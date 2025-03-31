# # Usa Node.js 18 en lugar de 14
# FROM node:18-alpine

# # Copia los archivos al contenedor
# COPY ./ ./ 

# # Instala dependencias
# RUN npm install

# # Comando por defecto
# CMD ["npm", "start"]
# Usa una versión más reciente de Node.js
FROM node:18-alpine

# Establece el directorio de trabajo
WORKDIR /app

# Copia los archivos package.json y package-lock.json antes de instalar dependencias
COPY package*.json ./

# Limpia la caché de npm y luego instala dependencias
RUN npm cache clean --force && npm install

# Copia el resto de los archivos
COPY . .

# Exponer el puerto
EXPOSE 8080

# Comando por defecto
CMD ["npm", "start"]