# Despliegue de un Sistema con Docker

# Instalación de un moodle y configuración básica para crear un curso y la agregación de usuarios

- Instalación con docker-compose 


### Correr localmente usando docker

1. Clonar el repositorio al directorio local de instalación

    $ git clone https://github.com/orlandoperez18/Despliegue-de-un-Sistema-con-Docker.git

![moodle-scree01](imagenes/paso%20uno.jpeg)

2. Para correr los contenedores

    $ cd Despliegue-de-un-Sistema-con-Docker/

    $ docker compose up

![moodle-scree02](imagenes/paso%20dos.jpeg)

3. Para solucinar los errores, detenemos los contenedores y hacemos unas configuraciones de grupo y de usuarios

    $ sudo chgrp docker mariadb_data/

    $ sudo chown 1001 mariadb_data/

![moodle-scree02](imagenes/errores.jpeg)

4. Ejecutamos de nuevo el comando

    $ docker compose up

![moodle-scree03](imagenes/errores-corregidos.jpeg)

5. Para verificar que los contenedores estan funcionando 

    $ docker ps -a

![moodle-scree04](imagenes/contenedores.jpeg)


# Paso 1) Correr Moodle y Login del web site

- http://localhost:90/
- Press Log In button

![moodle-scree05](imagenes/paso%20tres.jpeg)




# Paso 2) Login Moodle con Username y Password

Login with 
- Username: user
- Password: bitnani

![mooodle-screen06](imagenes/paso%20cuatro.jpeg)

### Dashboard inicial

![mooodle-screen06](imagenes/dashboard.jpeg)

# Paso 3) Creación de un curso

Nos dirigimos a 
- Site administration 
- Courses
- Add a new course

![mooodle-screen08](imagenes/paso-cinco.jpeg)

#
### Agreamos los datos que nosotros queremos que tenga el nuevo curso


![mooodle-screen09](imagenes/datos-cursos.jpeg)
#

### Visualización del nuevo curso ya creado

![mooodle-screen10](imagenes/curso-creado.jpeg)
#

# Paso 4) Cambios del perfil de administrador

Para realizar cambios para el administrador nos dirigimos "profile"

![mooodle-screen11](imagenes/admin.jpeg)
#

Despues de haber entrado en "profile", entramos en "edit profile"

![mooodle-screen12](imagenes/admin2.jpeg)
#

Despues de haber entrado en "edit profile", agregamos el nombre, apellido y correo del administrador

![mooodle-screen13](imagenes/admin3.jpeg)
#

Visualización de los cambios realizados a la cuenta del administrador

![mooodle-screen14](imagenes/admin4.jpeg)
#

# Paso 5) Creamos y agregamos al profesor al curso

Nos dirigimos a 
- Site administration 
- Users
- Add a new user

![mooodle-screen15](imagenes/usuarios.jpeg)
#

### Agreamos los datos del profesor

![mooodle-screen09](imagenes/datos-cursos.jpeg)
#