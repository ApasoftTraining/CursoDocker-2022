##Descargamos una versión concreta de UBUNTU, a través del tag
FROM ubuntu
MAINTAINER Apasoft Formacion "apasoft.formacion@gmail.com"
##Actualizamos el sistema
RUN apt-get update

##Instalamos nginx
RUN apt-get install -y nginx

##Instalamos apache
RUN apt-get install -y  apache2

##Creamos un lanzador para apache 
ADD apache.sh  /usr/local/bin/
RUN chmod +x /usr/local/bin/apache.sh

##Creamos un lanzador para nginx                                        
ADD nginx.sh /usr/local/bin/
RUN chmod +x /usr/local/bin/nginx.sh

## ponemos cualquier CMD, no es importante para el ejemplo
CMD ["echo", "prueba de comando"]

##Exponemos el Puerto 80
EXPOSE 80

