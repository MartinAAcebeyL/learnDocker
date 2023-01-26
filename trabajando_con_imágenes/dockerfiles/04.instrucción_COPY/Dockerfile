# Definimos el SO
FROM centos:7
# Instalamos apache para centos (S.O.)
RUN yum install -y httpd
# Copiamos la carpeta en el contenedor
COPY beryllium /var/www/html
# Ejecutamos Apache en primer plano
CMD apachectl -DFOREGROUND
# `docker build --tag apache-centos .`
# Nota no olvidar el punto final del comando 
# para referenciar el Docker file del directorio
# `docker images` para ver el listado de imagenes creadas

# `docker history -H apache-centos` para ver el historial 
# de capas del contenedor
# `docker run -d --name apache-centos -p 80:80 apache-centos` 
# para lanzar el contenedor en el puerto 80

# Got to: Localhost:80