# Definimos el SO
FROM ubuntu
# Instalamos apache para centos (S.O.)
RUN apt-get update \
    && apt-get install -y curl apt-utils wget unzip\
    && rm -rf /var/lib/apt/lists/*
# `docker build --tag apache-centos .`
# Nota no olvidar el punto final del comando 
# para referenciar el Docker file del directorio
# `docker images` para ver el listado de imagenes creadas