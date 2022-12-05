# ⚠🖥Proyecto - Computación Tolerante a Fallas 🖥⚠
En este repositorio se encuentra el proyecto final para la materia Computacion tolerante a fallas D06 Profesor: Michel Emanuel Lopez Franco.

![Aplicacion web que genera contraseñas](./images/inicio.png)

## Autores 📝🏻

* **Carbajal Armenta Yessenia Paola** 
* **Ortiz Perez Luis Alfonso** 
* **Sanchez Lozano Jonathan** 


## Herramientas🛠️

Elaborada con:

    Html
    Css
    Javascript

Tecnologias para el despliegue de la aplicación:
    
    Docker 
    OpenShift

## Descripción🔑
La aplicacion web es una aplicacion de generador de contraseñas, el usuario ingresa el tamaños de la cadena de caracteres, señala si puede incluir Mayúsculas, Minúsculas, Números y Símbolos, en ella se pueden obtener 4 diferentes niveles de "fuerza":

* **Muy Débil** 
* **Débil** 
* **Medio** 
* **Fuerte** 

![App inicial](./images/app.png)

Esta cuenta con varias validaciones como la dependencia de comparar que selecciones de casillas hace el usuario, si por ejemplo, selecciona pocos caracteres y pocas inclusiones de casillas esta será débil pero de igual forma se podrá generar.

![App inicial](./images/appdebil.png)

Por otro lado, si se selecciona una alta cantidad de caracteres y todas las casillas (o la mayoria), la contraseña que se generará será más fuerte.

![App inicial](./images/appfuerte.png)

Además de generar la contraseña, la app cuenta con la función de copiar en el portapapeles la contraseña mediante un botón, el cual se ubica dentro del recuadro donde se genera y que al hacerle clic aparece el mensaje de "copied".

![App inicial](./images/appcopie.png)


## Despligues🖥


### 🐳 Docker 🐳
Descargamos e instalamos Docker en el equipo:
https://www.docker.com/products/docker-desktop/
Seleccionamos el tipo de sistema operativo, una vez terminada la instalación nos pedirá reiniciar el equipo.
Abrimos CMD y comprobamos la instalación con: ``` docker versión ``` o ```docker –version```

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

##

### ⭕ OpenShift ⭕
Ingresamos a la página web de RedHat, creamos un perfil e ingresamos para usar DevSandBox.
https://developers.redhat.com/developer-sandbox

##

Una vez dentro del DevSandBox, nos posicionamos en la navegación como “Developer”.

![inicio sandbox](./images/inicio%20sandbox.png)


 
Una vez en la posicionados en la vista de “Developer” nos dirigimos a la sección de “Add” para agregar nuestra app que en esta ocasión será mediante la opción de “Git Repository”.

![sección add](./images/secci%C3%B3n%20add.png)
 
En esta pestaña añadimos la URL de nuestro repositorio de GitHub y así procedemos a crear nuestra app en OpenShift.

![importar git 1](./images/importar%20git%201.png)

![importar git 2](./images/importar%20git%202.png)

Ahora en la sección de “Topology” podemos ver que el deploy de nuestra app está listo y en ejecución.

![sección topology](./images/secci%C3%B3n%20topology.png)
 
Finalmente abrimos en otra pestaña nuestra app para comprobar que todo funciona de manera satisfactoria.
 
 ![deploy openshfit](./images/deploy%20openshift.png)


