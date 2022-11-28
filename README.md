# ⚠🖥Proyecto - Computación Tolerante a Fallas 🖥⚠
En este repositorio se encuentra el proyecto final para la materia Computacion tolerante a fallas D06 Profesor: Michel Emanuel Lopez Franco.

![Aplicacion web que genera contraseñas](./images/app.png)

## Autores 👋

* **Armenta Carbajal Yessenia Paola** 
* **Ortiz Perez Luis Alfonso** 
* **Sánchez Lozano Jonathan** 


## Descripción
La aplicacion web es una aplicacion de generador de contraseñas, el usuario ingresa el tamaños de a cadena de caracteres, señala si puede incluir Mayúsculas, Minúsculas, Números y Símbolos

Elaborada con:

    Html
    Css
    Javascript

Tecnologias para el despliegue de la aplicación:
    
    Docker 
    
## Despligue
Descargamos e instalamos Docker en el equipo:
https://www.docker.com/products/docker-desktop/
Seleccionamos el tipo de sistema operativo, una vez terminada la instalación nos pedirá reiniciar el equipo.
Abrimos CMD y comprobamos la instalación con: ``` docker versión ``` o ```docker –version```

### Docker
Creamos un archivo ‘Dockerfile’ (un archivo Docker que tendrá las nstrucciones necesarias para crear el entorno)

![Dockerfile](./images/dockfile.png)

Una vez que tu código esté listo y el Dockerfile está escrito, todo lo que tienes que hacer es crear tu imagen para contener tu aplicación.
```docker build -t "nombre:tag" .``` 

En nuestro caso:
```docker build -t html-server-image:v1 .```

![construccion](./images/construir.png)

Mostramos las imagenes de docker con
```docker images```

![imagenes](./images/imagenes.png)

Mostramos las imagenes de docker con
```docker images```

![imagenes](./images/imagenes.png)

Creada la imagen realizamos el lanzamiento:
```docker run -d -p 80:80 html-server-image:v1```

![despliegue](./images/despliegue.png)

En Docker desktop podemos realizar el despliegue de la siguiente manera:
1. Seleccionamos la imagen creada y la corremos

![imgaendesktop](./images/imagendesktop.png)

2. Seleccionamos el contenedor con la imagen de que creamos y damos click en el puerto 80:80

![contenedordesktop](./images/contenedordesktop.png)

Se habre el navegador web por defecto y nos aparece la aplicacion:

![puertos](./images/puertos.png)
