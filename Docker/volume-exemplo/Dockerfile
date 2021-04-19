# Imagem base  
FROM node:latest
# Autor
MAINTAINER Alisson Augusto
# Copiar tudo da pasta (Volume-exemplo) p/ pasta do container /var/www
COPY . /var/www
# Setar o diretório de trabalho (/var/www)
WORKDIR /var/www
# Instalar as dependências do projeto
RUN npm install
# Inicializa o container
ENTRYPOINT [ "npm", "start" ]
# Expõe a porta 3000
EXPOSE 3000

# Para buildar execute o comando na pasta deste projeto(volume-exemplo): 
# docker build -f Dockerfile -t alisson/node .
# onde -t indica a tag alisson/node
# . indica a pasta atual


# exemplo de variaveis de ambiente
# ENV PORT=3000
# EXPOSE $PORT