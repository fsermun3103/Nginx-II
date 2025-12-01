# Project Name
### Nginx-II

# Authors Name
### Ángel Ortega - Francisco José Serrano

## Creación de dos usuarios cons sus contraseñas en /etc/nginx/.htpasswd
![Creación de dos usuarios](/doc/creacion-usuarios.png)

## Configuración del servidor para usar la autenticación básica
![Configuración de autenticación](/doc/config-autenticacion.png)

## Prueba de la página http://paco.test

#### Al principio me salía un error 403 Forbidden, y por eso cree un index.html en la carpeta /var/www/paco.test/html
#### Me pide correctamente el login
![Prueba autenticación](/doc/prueba-autenticación.png)

#### Pruebo a entrar con un usuario y contraseñas erróneos y se comporta correctamente
![Error Autenticación](/doc/error-autenticación.png)

#### Pruebo el acceso con el usuario y contraseña correctos y me saca correctamente el index.html que cree
![Acceso correcto](/doc/acceso-correcto.png)

## Muestro un log de error y otro de acierto en ese orden
![Logs error y acierto](/doc/logs-error-acierto.png)

## Cambio /etc/nginx/sites-available/paco.test para que solo me pida autenticación en contact.html
![Autenticación solo en contact.html](/doc/autenticación-contact.html.png)

#### Funciona correctamente
![Contact autenticacion](/doc/contact-autenticacion.png)

## Cambio el archivo paco.test para que me pida la autenticación básica y restrinja las ips indicadas
![Cambio paco.test](/doc/autenticacion-básica-y-restriccion-ip.png)

## Cambio el archivo paco.test para que restrinja mi ip 192.168.56.1
![Cambio paco.test](/doc/restringir-ip.png)

#### Ahora cuando intento acceder a la página me muestra el error 403 Forbidden
![403 Forbidden](/doc/403-mi-ip.png)

#### Este es el error.log que se me genera cuando intento acceder
![error.log](/doc/error.log.png)

## Configuración final de paco.test para que salte la autenticación en la página principal
## Y además comprueba que tengas una ip válida
![paco.test final](/doc/paco.test-final.png)

#### Ahora me salta la validación en la página principal y funciona correctamente