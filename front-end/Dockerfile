# Use uma imagem Node.js com servidor web integrado
FROM node:18-alpine

# Instala o servidor web simples
RUN npm install -g http-server

# Define o diretório de trabalho
WORKDIR /app

# Copia os arquivos do frontend
COPY index.html .
COPY style.css .
COPY script.js .

# Expõe a porta 8080
EXPOSE 8080

# Comando para iniciar o servidor
CMD ["http-server", "-p", "8080", "--cors"]
