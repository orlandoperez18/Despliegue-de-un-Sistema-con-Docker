# Despliegue de un Sistema con Docker

# Instalación de un moodle y configuración básica para crear un curso y la agregación de usuarios

- Instalación con docker-compose 


### Correr localmente usando docker

1. Clonar el repositorio al directorio local de instalación

    $ git clone https://github.com/orlandoperez18/Despliegue-de-un-Sistema-con-Docker.git

![moodle-scree01](imagenes/paso%20uno.png)

2. Para correr los contenedores

    $ cd Despliegue-de-un-Sistema-con-Docker/

    $ docker compose up

![moodle-scree02](imagenes/paso%20dos.png)

3. Para solucinar los errores, detenemos los contenedores y hacemos unas configuraciones de grupo y de usuarios

    $ sudo chgrp docker mariadb_data/

    $ sudo chown 1001 mariadb_data/

![moodle-scree02](imagenes/errores.png)

4. Ejecutamos de nuevo el comando

    $ docker compose up

![moodle-scree03](imagenes/errores-corregidos.png)

5. Para verificar que los contenedores estan funcionando 

    $ docker ps -a

![moodle-scree04](imagenes/contenedores.png)


# Paso 1) Correr Moodle y Login del web site

- http://localhost:90/
- Press Log In button

![moodle-scree05](imagenes/paso%20tres.png)




# Paso 2) Login Moodle con Username y Password

Login with 
- Username: user
- Password: bitnani

![mooodle-screen06](imagenes/paso%20cuatro.png)

### Dashboard inicial

![mooodle-screen06](imagenes/dashboard.png)

# Paso 3) Creación de un curso

Nos dirigimos a 
- Site administration 
- Courses
- Add a new course

![mooodle-screen08](imagenes/paso-cinco.png)

#
### Agreamos los datos que nosotros queremos que tenga el nuevo curso


![mooodle-screen09](imagenes/datos-cursos.png)
#

### Visualización del nuevo curso ya creado

![mooodle-screen10](imagenes/curso-creado.png)
#

# Paso 4) Cambios del perfil de administrador

Para realizar cambios para el administrador nos dirigimos "profile"

![mooodle-screen11](imagenes/admin.png)
#

Despues de haber entrado en "profile", entramos en "edit profile"

![mooodle-screen12](imagenes/admin2.png)
#

Despues de haber entrado en "edit profile", agregamos el nombre, apellido y correo del administrador

![mooodle-screen13](imagenes/admin3.png)
#

Visualización de los cambios realizados a la cuenta del administrador

![mooodle-screen14](imagenes/admin4.png)
#

# Paso 5) Creamos y agregamos al profesor al curso

Nos dirigimos a 
- Site administration 
- Users
- Add a new user

![mooodle-screen15](imagenes/usuarios.png)
#

### Agreamos los datos del nuevo profesor

![mooodle-screen16](imagenes/profesor.png)
#

Para darle el rol de profesor debemos de entrar a nuestro curso y en el apartado de "participants" le damos click para agregar "Enrol Users"

![mooodle-screen17](imagenes/roldeprofe.png)
#

Agregamos al usuario y le asignamos el rol de "Teacher"
![mooodle-screen18](imagenes/enrol.png)
#

# Paso 6) Creamos y agregamos a los estudiantes al curso

Nos dirigimos a 
- Site administration 
- Users
- Add a new user

![mooodle-screen15](imagenes/usuarios.png)
#

### Agreamos los datos de cada alumno

Datos del primer alunmno
![mooodle-screen19](imagenes/alumno1.png)
#

Datos del segundo alunmno
![mooodle-screen20](imagenes/alumno2.png)
#

Datos del tercer alunmno
![mooodle-screen21](imagenes/alumno3.png)
#

Para darle el rol de profesor debemos de entrar a nuestro curso y en el apartado de "participants" le damos click para agregar "Enrol Users"

![mooodle-screen17](imagenes/roldeprofe.png)
#

Agregamos a los usuarios y le asignamos el rol de "Students"
![mooodle-screen22](imagenes/students.png)
#
