# 💥🐒Chaos Monkey🐒💥

<p align="justify">
  Chaos Monkey es una herramienta software que de forma aleatoria detiene instancias y contenedores que están ejecutándose en el entorno de producción. El objetivo es exponer a los sistemas a fallos para ayudar a los ingenieros a proveer servicios que sean capaces de reaccionar a caídas y otros problemas inesperados.

 * **Chaos Engineering es la disciplina de experimentar en un sistema para generar confianza en la capacidad del sistema para soportar condiciones turbulentas en la producción.** 
</p>

##

<p align="center">
  <img src="https://i.pinimg.com/originals/52/ce/57/52ce57e7e3cbb5a31cc7792180d734d9.gif">
</p>

##

## Online tool de Chaos Monkey🖥️💥

<p align="justify">
  Esta herramienta es una interfaz gráfica en donde se puede simular el caos del mono con ayuda de diversos factores como servidores, apps, peticiones y ataques virtuales el cual se usa para probar el sistema en la nube.
</p> 

##
<p align="justify">
  1.- Comenzamos registrando una instancia EC2.
</p> 

<p align="center">
  <img src="/images/1.png">
</p>

<p align="justify">
  2.- Llenamos los datos del formulario para crear la instancia.
</p> 

<p align="center">
  <img src="/images/2.png">
</p> 

<p align="justify">
  3.- Seleccionamos los servicios que queremos que tenga nuestra instancia dando clic en las casillas.
</p> 

<p align="center">
  <img src="/images/3.png">
</p> 

<p align="justify">
  4.- Añadimos un servicio que no está listado en la sección de add el cual se llamará FooService.
</p> 

<p align="center">
  <img src="/images/4.png">
</p> 

<p align="justify">
  5.- Ahora, aquí podemos ver los servicios que tiene nuestra máquina al desplegarlos en la sección de + y proseguimos añadiendo 4 máquinas más.  
</p>

<p align="center">
  <img src="/images/5.png">
</p> 

<p align="justify">
  6.- Comenzamos a crear la red.
</p>

<p align="center">
  <img src="/images/6.png">
</p> 

<p align="justify">
  7.- Le damos un nombre a la red.
</p>

<p align="center">
  <img src="/images/7.png">
</p> 

<p align="justify">
  8.- Posteriormente, añadimos a la red todas las máquinas que creamos en nuestra instancia.
</p>

<p align="center">
  <img src="/images/8.png">
</p> 

<p align="justify">
  9.- Al crearla, veremos algo así y proseguimos a dar clic en el botón de la computadora en Actions para conectarlas.
</p>

<p align="center">
  <img src="/images/9.png">
</p> 

<p align="justify">
  10.- Seguimos conectando las máquinas de la red.
</p>

<p align="center">
  <img src="/images/10.png">
</p> 

<p align="justify">
  11.- Ahora seguimos en la sección de Perf and Load Test, iniciando como primer paso con las credenciales del usuario.
</p>

<p align="center">
  <img src="/images/11.png">
</p> 

<p align="justify">
  12.- En el segundo paso nos encontramos con el número de instancias que queremos usar, el URL que vamos a testear y finalmente con el número de peticiones que haremos a ese sitio.
</p>

<p align="center">
  <img src="/images/12.png">
</p> 

<p align="justify">
  13.- En seguida, en este tercer paso el sistema nos ayudará a lanzar las 10 instancias online que pusimos en el paso anterior, las cuales están listas para atacar.
</p>

<p align="center">
  <img src="/images/13.png">
</p> 

<p align="justify">
  14.- Como cuarto y último paso podremos ver la respuesta en tiempo real de las peticiones al sitio.

<p align="center">
  <img src="/images/14.png">
</p>





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
