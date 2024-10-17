1-Descarga la imagen 'httpd' y comprueba que está en tu equipo.

--sudo docker pull httpd

--sudo docjer images

2-Crea un contenedor con el nombre 'dam_web1'.

--sudo docker run --name=dam_web1 httpd /bin/sh

3-Si quieres poder acceder desde el navegador de tu equipo, ¿que debes hacer?

Tienes que escribir en el navegador 10.0.9.144

Utiliza bind mount para que el directorio del apache2 'htdocs' esté montado un directorio que tu elijas. 

--sudo docker run -p 8080:80 -v /home/daniel/Compartida:/usr/local/apache2/htdocs --name dam_web1 httpd

4-Realiza un 'hola mundo' en html y comprueba que accedes desde el navegador.

<html>
  <head></head>
  <body>
    <h1>Hola mundo</h1>
  </body>
</html>

Tienes que escribir en el navegador 10.0.9.144
