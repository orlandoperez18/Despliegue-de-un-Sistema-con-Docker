# Despliegue de un Sistema con Docker

# Instalación de un moodle y configuración básica para crear un curso

- Instalación con docker-compose 


### Correr localmente usando docker

1. Clonar el repositorio al directorio local de instalación
git clone https://github.com/orlandoperez18/Despliegue-de-un-Sistema-con-Docker.git

2. Para correr los contenedores

$cd moodle

$docker compose up

3. Para detener los contenedores

$docker compose down


# Paso 1) Correr WordPress y Configurar

- http://localhost:8000/
- Configure Site Title e.g. WCMX
- Username e.g. admin
- Password e.g. 123456 
- Confirm Password checked
- Press Install Button

![WordPress-Screen01](imgs/01WP_Install.png)

# Paso 2)Login del web site

- Press Log In button

![mooodle-screen1](imagenes/uno.png)

# Paso 3) Login WordPresss con Username y Password

- Login with Username user
- Password bitnani

![WordPress-Screen03](imgs/03WP_Install.png)

# Paso 4) Seleccionar Menu Pluggins

- Select Option Pluggins

![WordPress-Screen04](imgs/04WP_DeletePluggins.png)

# Paso 5) Agregar Pluggins

- Add Pluggin Guttentor 
- Select Guttentor pluggin and press Install Now

![WordPress-Screen05](imgs/05WP_AddPluggins.png)

# Paso 6) Agregar Pluggins

- Add Pluggin Classic Editor
- Select Button Activate

![WordPress-Screen06](imgs/06WP_AddPluggins.png)

# Paso 6) Agregar Pluggins

- Add Pluggin Addons for Gutenberg
- Select Instal Now
- Select Button Activate

![WordPress-Screen07_2](imgs/07_2WP_AddPluggins.png)


# Paso 7) Configurar Block editor

- Select Settings
- Choose Block editor
- Button Save Changes

![WordPress-Screen07_3](imgs/07_3WP_AddPluggins.png)

# Paso 8) Agregar un Tema

- Select Appereance Menu
- Choose Add New Theme
- Search Ample Bussiness Epic
- Add Theme

![WordPress-Screen07](imgs/07WP_AddPluggins.png)

# Paso 8) Importar una Pagina

- Menu Tools
- Select Upload file and import
- Choose wcmx.WordPress.2020-08-10.xml file


![WordPress-Screen08](imgs/08Import.png)

# Paso 9) Editar un Post

- Esto importa el ejemplo pero no la media (imagenes)

![WordPress-Screen09](imgs/09Import.png)


# Paso 10) Editar Post

- Select Posts Menu
- Select Test 2 Post

![WordPress-Screen10](imgs/10EditPosts.png)


# Paso 11) Agregar Media a Post 2

- Select Post and Button Edit Image
![WordPress-Screen11](imgs/11WP_AddPhotos.png)

- Upload images carrusel01-1.jpg carrusel02.jpg carrusel03.jpg
![WordPress-Screen12](imgs/12WP_AddPhotos.png)

- Select image for other post
![WordPress-Screen13](imgs/13WP_AddPhotos.png)