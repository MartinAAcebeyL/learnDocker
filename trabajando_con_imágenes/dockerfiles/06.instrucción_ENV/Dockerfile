# Definimos el SO
FROM centos:7

# Instalamos apache para centos (S.O.)
RUN yum install httpd -y
# ENV <variable-name> <variable-value>
ENV contenido <h1>Contenido de la variable</h1>
# RUN echo incluye el valor de la variable dentro 
# del archivo indicado
RUN echo "$contenido"> /var/www/html/prueba.html

# Ejecutamos Apache en primer plano
CMD apachectl -DFOREGROUND
# `docker build --tag apache-centos:env .`
# construimos la imagen incluyendo un nuevo tag

# Nota no olvidar el punto final del comando 
# para referenciar el Docker file del directorio

# `docker images` para ver el listado de imagenes creadas

# `docker history -H apache-centos` para ver el historial 
# de capas del contenedor

# matamos el contendor activo anterior `apache-centos`
# `docker rm -fv apache-centos`

# `docker run -d --name apache-centos-env -p 80:80 apache-centos:env` 
# para lanzar el contenedor en el puerto 80

# Got to: Localhost:80/prueba.html    o    http://localhost/prueba.html