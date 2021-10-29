# GitHub 
_**Autor:** Leonardo Di Mauro. 24/09/2021_

## ¿Qué es [GitHub](www.github.com)? 
Github es un portal creado para alojar el código de las aplicaciones de cualquier desarrollador.

La plataforma está creada para que los desarrolladores suban el código de sus aplicaciones y herramientas, y que como usuario no sólo puedas descargarte la aplicación, sino también entrar a su perfil para leer sobre ella o colaborar con su desarrollo.

A continuación veremos como crear un nuevo proyecto, subir un archivo al servidor de GitHub y dar permiso a un colaborador para que pueda editar los archivos con la finalidad de corregirlos o añadir mas información.

### Paso 1:
* Entramos a [GitHub](www.github.com), nos registramos y creamos un **Nuevo Proyecto**.
* Ponemos un nombre al nuevo repositorio y una descripción.
* Indicamos que el repositorio sea **Público** para que sea visible por cualquiera. En caso contrario marcamos **Privado**.
* Seleccionamos el _checkbox_ para crear automáticamente un archivo **README.md** que podremos modificar más adelante.

### Paso 2:

* Abrimos terminal en Linux, nos situamos en la carpeta donde queremos que se clone el repositorio y ejecutamos el comando **git clone** + la **_url_** del repositorio de la siguiente manera:
```
$ git clone https://github.com/LeonardoDiMauro/Proyecto-java
```
* Nos pedirá **_nombre de usuario_** y **_token_**, usaremos el nombre que indicamos en el registro y el token lo encontraremos en la web de GitHub, pinchamos en la imagen de nuestro usuario, luego click en **_settings_** -> **_developer settings_** -> **_personal access tokens_** -> **_generate new token_**.
* Creamos un archivo de pruebas, por ejemplo: test.java o quizas un holamundo.txt y una vez escrito lo guardamos.
* Luego ejecutamos en la terminal:
$ git add .
$ git config user.email "dima65100@gmail.com"
$ git config user.name "LeonardoDiMauro"
* Añadimos un comentario o _commit_ con:
$ git commit -m "primer comentario"
* Lo enviamos al server de GitHub con el siguiente comando (Nos volvera a pedir **_nombre de usuario_** y **_token_**).
$ git push
* Nuestro archivo ya esta disponible para ser editado por un colaborador autorizado por nosotros.

### Paso 3:

* Para que otro usuario pueda modificar los archivos de nuestro repositorio será necesario enviarle una **invitación**, esto se hace pinchan
Esa persona tiene que enviarnos una invitación, para enviar la invitación debemos estar situados en el **home** de GitHub, en la esquina superior izquierda estarán listados nuestros repositorios. Pinchamos en el que queremos compartir -> **_settings_** -> **_manage access_** -> **_invite a collaborator_**.
* Abrimos terminal en Linux y nos situamos en el directorio donde queremos trabajar.
* El colaborador nos enviara la **_url_** de su repositorio, entonces ejecutamos el siguiente comando en la terminal:
$ git clone https://github.com/RedSalazar/PorParejas
* Entramos en la carpeta:
$ cd PorParejas
* Editamos el archivo que queramos:
$ gedit prueba.java
* Hacemos los cambios oportunos, guardamos y subimos al servidor de GitHub con el comando:
$ git add .
$ git config user.email "dima65100@gmail.com"
$ git config user.name "LeonardoDiMauro"
* Añadimos un comentario o _commit_ con los cambios realizados:
$ git commit -m "modificado, faltaba un ;"


### Bibliografia:

* https://www.xataka.com/basics/que-github-que-que-le-ofrece-a-desarrolladores
* https://kinsta.com/es/base-de-conocimiento/que-es-github/
* 
### Conclusiones:

GitHub es un sistema que permite trabajar a varios usuarios al mismo tiempo en un mismo proyecto. Permite ademas llevar un control con fecha y hora sobre quien ha moficado archivos y que cambios a realizado, con la posibilidad de volver atras en caso de sea necesario.
