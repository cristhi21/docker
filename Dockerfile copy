FROM node:12
#Copiar todos los archivos del directorio . a la ruta "/usr/src/ dentro de nuestro contenedor
#Contexto de build
COPY [".", "/usr/src/"]
#Directorio de trabajo dnetro del contexto de build
WORKDIR /usr/src
#Dependencias de node
RUN npm install
#Exponer un puerto, nos sirve para acceder a un contenedor en nuestra maquina anfitriona a travez de este puerto
EXPOSE 3000
#Proceso por defecto que se va a ejcutar si no especificamos un proceso al hacer docker run 
CMD ["node", "index.js"]
