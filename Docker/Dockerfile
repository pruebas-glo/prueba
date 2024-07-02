# Usa la imagen base de Apache HTTP Server para ARM64 con una etiqueta específica
FROM arm64v8/httpd:2.4.51-alpine

# Copia el archivo index.html al directorio de trabajo en la imagen
COPY index.html /usr/local/apache2/htdocs/

# Puerto en el que escuchará Apache
EXPOSE 80

# Comando para iniciar Apache cuando se ejecute el contenedor
CMD ["httpd", "-D", "FOREGROUND"]
