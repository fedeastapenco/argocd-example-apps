# Usamos Node.js 20 slim para ligereza
FROM node:22-slim

# Directorio de trabajo
WORKDIR /app

# Copiamos package.json + package-lock.json para instalar deps
COPY package*.json ./

# Instalamos dependencias
RUN npm install --production

# Copiamos el código de la aplicación
COPY . .


# Comando por defecto
CMD ["node", "ticket-generator.js"]
