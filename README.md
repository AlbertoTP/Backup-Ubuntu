# Respaldo de mi S.O. Linux - Kubuntu (Ubuntu 16.04.3 LTS)

Archivos del respaldo utilizar Aptik para restaurar

## Aptik
Aptik es una utilidad que nos permite simplificar la reinstalación de paquetes en una instalación limpia de Ubuntu.

#### ¿Qué nos permite guardar y recuperar Aptik?

* Repositorios PPA (Software Sources PPA) nos permitirá volver a instalar todos los repositorios que hayamos añadido.
* Paquetes descargados (Downloaded Packages) nos permitirá recuperar los paquetes .deb que hayamos instalado y estén en la ruta /var/cache/apt/archives, lo que vendrá especialmente bien para cuando instalemos software de fuera de repositorios.
* Paquetes de software (Instaled Software) nos permitirá guardar y recuperar todos los paquetes que hayamos instalado después de la instalación del sistema.
* Temas e iconos (Themes and Icons) nos permitirá guardar y recuperar los temas e iconos GTK o KDE que tengamos instalados y estén en las rutas /usr/share/icons y /user/share/themes.
* Sistemas de archivos (Filesystem Mounts) nos permitirá guardar y recuperar configuraciones de carpetas de archivos de aplicación comprimidas del directorio personal.
* Usuarios y Grupos (Users and Groups) nos permitirá guardar y recuperar, como su nombre indica, usuarios y grupos, lo que incluye las contraseñas de acceso, miembros de grupos, etc.
* Ajustes de aplicaciones (Applications Settings) nos permitirá guardar y recuperar los ajustes de aplicaciones, lo que significa que todos los cambios que hubiéramos hecho en ellas seguirán estando ahí.
* Datos de la carpeta personal (Home Directory Data) nos permitirá guardar y recuperar el contenido de nuestra carpeta personal. Aunque es una opción, para esto yo recomendaría crear y usar la partición /home.
* Tareas programadas (Scheluded Tasks) nos permitirá guardar y recuperar las entradas de la pestaña cron para todos los usuarios.

## Instalar Aptik

Para instalar Aptik en tu sistema, abre una terminal y añade el siguiente repositorio:

```{r, engine='bash', count_lines}
sudo apt-add-repository -y ppa:teejee2008/ppa
sudo apt-get update
sudo apt-get install aptik
```


[Aqui se puede encontrar más información](https://ubunlog.com/aptik-herramienta-copias-seguridad/)



## Para verificar la versión de Ubuntu:

```{r, engine='bash', count_lines}
lsb_release -a
```
