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