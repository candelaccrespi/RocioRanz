# Resumen

## En este documento se documentarán algunos de los puntos aprendidos durante el curso según se detalla en la explicación de la prueba final publicada en Aula Global.

### Instalación de un programa de emulación de la terminal

En mi caso, el programa en cuestión fue, en primer lugar, **Git Bash**, debido a que no conseguí que Ubuntu funcionase en mi ordenador. Sin embargo, durante el curso, el profesor indicó que era más recomendable que utilizásemos **Cygwin**. Es por ello que lo instalé desde la página web y sin complicaciones. Entramos en la [página web de Cygwin](http://cygwin.com) y le dimos a instalar. Instalamos (mediante una búsqueda) los siguientes paquetes: **libcurl4, wget, ca-certificates-letsencrypt, lynx, nano, openssl (este suele venir ya)**. Para instalarlo, en la columna de “New”, le damos a la flecha de nuestro paquete y marcamos la última
opción/versión.Seleccionamos los ajustes, metiéndolo en un directorio temporal en el que sería instalado, descargamos los paquetes de software seleccionando cuáles queríamos y esperamos a que se completase el proceso. 

### Configuración del programa

Para emular la terminal, es necesario tener un destino. En este caso, durante el curso, nos hemos centrado en conseguir clonar archivos de nuestra propia terminal (primero delante Git Bash y luego mediante Cygwin) a Github. Por ello, el primer paso a dar era **clonar el repositorio** que habríamos creado en Github a nuestra propia terminal para tener una conexión directa. Este paso se realizó mediante el comando **git clone https://github.com/rocioranz/practicas-periodismo-de-datos**, mi ruta. Además, fue necesario, por supuesto, configurar desde Git Bash, y luego Cygwin, nuestro nombre de usuario y contraseña de GitHub. Para ello tuvimos que escribir **git config --global user.rocioranz** , y luego **git config --global user.100386359@alumnos.uc3m.es**. Después, como siempre, **git commit** para guardar los cambios. Habiendo hecho esto comprobamos que todo se había guardado con éxito desde **git status**. 

*Inciso: datos básicos que aprendimos al principio del curso fue a configurar "micasa" y a hacer **pwd** para ver dónde nos hallábamos y **cd** para movernos por nuestras carpetas, con **ls** para ver todo lo contenido en cada carpeta*

### Configuración de un programa de edición de texto

En nuestro caso, hemos utilizado Nano. Nano ya venía dentro de Cygwin (hemos comentado antes que especificamos al instalar Cygwin que nano también se instalase con éxito), algo que podemos comprobar porque al introducir el comando de su nombre, **nano**, se abría. La configuración que llevamos a cabo fue conseguir que apareciesen los números de línea mediante el comando **set linenumbers**. También habilitamos una sangría automática puesto que nano no la tiene y es muy incómodo escribir en líneas que continúan hacia la derecha y no terminan. Para ello ejecutamos **set autoindent** y conseguimos tener líneas en las que la visualización fuera mucho más sencilla.

### Versión del lenguaje de SHELL utilizado.

Se comprende que, siendo compatible con Cygwin, se ha utilizado el shell de Hamilton C, que es un shell de Windows muy similar al shell de Unix C. Microsoft distribuyó Windows Services para UNIX para su uso con sus sistemas operativos basados en NT en particular, que tienen un subsistema ambiental POSIX.

### Valor de la variable de entorno PATH.

En primer lugar, es necesario recordar que una variable de entorno es, simplemente, una parte del entorno, como su nombre indica, en que se ejecuta un proceso. Son dinámicas y permiten continuar con el sentido del mismo. Las variables de entorno empiezan por el símbolo $, que no hay que confundir el que aparezca a principio de la línea. Por ejemplo, $HOME significa la ruta de nuestro usuario. $PATH nos muestra las rutas donde están los programas que se puedan ejecutar. Para consultar, usamos echo. echo $PATH nos muestra las rutas. 

### Comandos utilizados y ejemplos.

Algunos de los comandos aprendidos durante el curso:

- ls → ver qué archivos y carpetas hay en la ruta en la que estamos). 
- cd → entrar a una carpeta específica. 
- pwd → para saber en qué ruta estamos actualmente.
- mkdir → crear una carpeta nueva especificando su nombre.
- mv → mover o renombrar archivos o directorios. [origen] [destino]
- && → sirve para ejecutar dos comandos en una misma línea o de una vez. 
- man → este comando es el de “manual”, el que nos dice qué hace un comando y nos muestra todas las opciones posibles. Por ejemplo, si queremos saber qué hace ls y qué opciones podemos usar (como que nos especifique quién es el propietario de un archivo o carpeta), tenemos que usar man ls.
- cat → sirve para previsualizar en la propia terminal el archivo. 
- mkdir para crear directorios
- nano para editar los textos
- git add para añadir elementos
- git commit para ejecutarlo
- git push para subirlo 

Mejor que aportar ejemplos aleatorios con cada comando, he preferido incluir explicaciones detalladas previamente para que se vea cuándo han sido utilizados, dejando que el ejemplo sea el aprendizaje mismo. 

# RocioRanz
