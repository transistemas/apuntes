![LogoTransistemas](https://github.com/transistemas/apuntes/blob/master/archivos/logo-transistemas.svg)


# GIT 

## MANEJAR REPOSITORIOS

![Logo](https://miro.medium.com/max/910/1*BCZkmZR1_YzDZy22Vn4uUw.png)


## Instalar GIT
**En windows:**

- Instalar GITBASH. 
 [GitBash](https://gitforwindows.org/)
 
**En linux (Linux Mint, Fedora, Ubuntu, Debian, etc)**

Abrir la terminal y correr el siguiente comando: 

- Ubuntu: 	

	*sudo apt update*

	*sudo apt install git*


- Fedora: 	

	*sudo dnf update*

	*sudo dnf install git*


- Otras distribuciones:

	*sudo yum -y update*

	*sudo yum install git*

Para chequear que se instaló correctamente ejecutamos en la consola:

*git --version*

y nos tiene que aparecer la versión de git que se instaló en nuestra computadora.

## ¿Cómo crear un repositorio desde cero?

En github entramos con nuestro usuario, vamos a la parte de repositorios y hacemos click en NEW

![newrepo1](https://github.com/transistemas/apuntes/blob/master/archivos/tutorialgit/newrepo1.jpg)


Luego nos va a aparecer esta ventana, donde podemos poner el nombre del repo (es una buena práctica poner el nombre del proyecto como nombre de repositorio), si es público o privado y si queremos que inicie con un archivo llamado readme (que es aconsejable que los proyectos de sistemas tengan un readme, pero no es obligatorio). Y le damos click a “create repository”


![newrepo2](https://github.com/transistemas/apuntes/blob/master/archivos/tutorialgit/newrepo2.jpg)


Una vez creado entramos en nuestra terminal a la carpeta donde vamos a tener localmente nuestros archivos para vincular con el repositorio.

(Para entrar a un carpeta de nuestra computadora desde una terminal usamos el comando “cd”, escribimos cd y la ruta de la carpeta a la que queremos entrar, ejemplo: “cd d:/miCarpeta/repos”)

![newrepo3](https://github.com/transistemas/apuntes/blob/master/archivos/tutorialgit/newrepo3.JPG)


Una vez que estamos en la carpeta que deseamos vamos a ejecutar todos los comandos que se nos desplegaron en github al crear el repo:

![newrepo4](https://github.com/transistemas/apuntes/blob/master/archivos/tutorialgit/newrepo4.JPG)

### ¿Cómo crear un repositorio desde cero?

*git init*
(Inicializa nuestra carpeta como un repositorio git, esto es necesario la primera vez solamente)

*git add README.md*
(Con este comando agregamos los archivos que queremos subir)

*git commit -m "first commit"*
(Prepara el paquete de archivos que se van a subir y las vincula al branch donde estamos parados)

*git remote add origin https://github.com/caru08/miRepositorio.git*
(Le indica a nuestra carpeta local cuál va a ser el repositorio de github con el que se va a vincular)

*git push -u origin master*
(Sube los cambios del commit al repositorio en la nube)



## ¿Cómo obtener un repositorio que ya existe?

Necesitamos la url url del repositorio al que me quiero unir:
Ejemplo: https://github.com/joseCaceres086/transistemas-web

En la consola nos paramos en la carpeta donde queremos que este nuestro proyecto, usamos el comando “cd” para entrar en la carpeta que queremos.

(Para entrar a un carpeta de nuestra computadora desde una terminal usamos el comando “cd”, escribimos cd y la ruta de la carpeta a la que queremos entrar, ejemplo: “cd d:/miCarpeta/repos”)


Y ejecutamos el comando *clone*:

*git clone https://github.com/joseCaceres086/transistemas-web.git*

![newrepo5](https://github.com/transistemas/apuntes/blob/master/archivos/tutorialgit/newrepo5.JPG)


## Comandos utiles:

**git status**

Me permite ver que archivos fueron modificados con respecto a lo que está en el repositorio de la nube. Me va a aparecer en rojo lo que no esté agregado al paquete para commitear y en verde lo que esté agregado (va a aparecer en verde todo lo que haya agregado con *git add nombrearchivo.html*)

![newrepo6](https://github.com/transistemas/apuntes/blob/master/archivos/tutorialgit/newrepo6.JPG)


**git reset**

Me permite quitar archivos agregados con el add para el commit. Pongo *git reset* más el nombre del archivo que quiero quitar. Ejemplo: *git reset miarchivo.html*

![newrepo7](https://github.com/transistemas/apuntes/blob/master/archivos/tutorialgit/newrepo7.JPG)


**git pull**

Me permite bajar los cambios que están en el repositorio de la nube a mi repositorio local. Si no hay cambios me va a aparecer “already up to date”

![newrepo8](https://github.com/transistemas/apuntes/blob/master/archivos/tutorialgit/newrepo8.JPG)


**git branch**

Me muestra la lista de branchs que existen en mi repositorio local (el que aparece en verde es en el que estoy parado).
Si le agrego *git branch -a* me muestra tanto los locales como los del repositorio del github. 




