# ejemplored
<p align="center">
 <img src="https://unsplash.com/es/fotos/MAYEkmn7G6E" alt="imagen portada">
</p> 
<h1 align="center">Readme de Git y GitHub</h1>
 
<h3>Introducción</h3>
<p>En este README te explicaré mi experiencia y los pasos que tuve que tomar para instalar y configurar Git y GitHub, ya que son esenciales para tu desarrollo educativo y desempeño profesional, una forma popular de crear y revisar código. Partiendo de los principales conceptos.

¿Qué es el control de versiones?
Es un software capaz de registrar los cambios realizados en un archivo a lo largo del tiempo, de modo que puedas recuperar versiones específicas más adelante. Es un instrumento útil para un diseñador gráfico, desarrollador web o ingeniero/a.

Existen tres tipos de sistemas de control de versiones:
* Local
* Centralizado
* Distribuido


*Git*
Se le conoce al sistema de control de versiones (Control Versión System o CVS) y de código abierto. Fue creado por Linus Torvals en 2005.
Para usar git se necesita alojarlos en repositorios. Un repositorio es un proyecto que contiene múltiples archivos. Hay dos maneras para alojar los repositorios: primero es en línea (en la nube) y la segunda es fuera de línea (auto-instalado en tu servidor). El más popular es GitHub.

*Github:*
Aquí se aloja ese código y sus cambios en un servidor en la nube, así como ver el código de otras personas que tiene sus repositorios públicos. Es el hub para guardar todos mi git. 

¿Por qué lo necesitamos?
- Documentación: facilita la obtención de excelente documentación
- Opciones de Integración: en plataformas como Amazon, Google Cloud, Code Climate 
- Rastrea cambios de código a través de versiones: seguimiento de todos los cambios que se han enviado al repositorio 
- Muestra tu trabajo
</p>

-------------------------------------------------------------------------------------------------------------------------------------------
<h3>Instalar Git en macOS</h3>

Git es el responsable de todo lo relacionado con GitHub que ocurra localmente en el equipo, por ello es necesario descargar, instalar y configurar Git en tu equipo.    
Para instalar Git en macOS simplemente es necesario descargar un instalador binario. La dirección del instalador la puedes obtener desde la página de descargas de Git para macOS.    
Redirigete al sitio de descarga del instalador.   
Debes hacer click en el botón Download para iniciar la descarga. Instale la versión  más reciente de Git. 

Una vez la descarga concluya es necesario ejecutar el instalador y seguir los pasos del asitente para terminar la instalación.


<h3>Configurar Git</h3>

Ahora que tienes Git en tu sistema, vas a querer hacer algunas cosas para personalizar tu entorno de Git. Es necesario hacer estas cosas solamente una vez en tu computadora, y se mantendrán entre actualizaciones. También puedes cambiarlas en cualquier momento volviendo a ejecutar los comandos correspondientes.

1. Utiliza la terminal e ingresa el comando *git config* 
2. Establece el nombre de usuario en Git, con el comando *git config --global user.name "Lai Doe"* 
3. Establece la dirección de correo electrónico de confirmación en Git, con el comando *git config --global user.email laidoe@gmail.com*

Ahora que tu identidad esta configurada, puedes elegir el editor de texto por defecto que se utilizará cuando Git necesite que introduzcas un mensaje. Si no se indica nada, Git usará el editor por defecto de tu sistema, que generalmente es Vim. 

<h4>Comprobando tu configuración</h4>  

Usa el comando *git config --list*

También puedes comprobar el valor que Git utilizará para una clave específica ejecutando *git config <key>*

-------------------------------------------------------------------------------------------------------------------------------------------
<h3>Autenticación con GitHub desde Git</h3>
Cuando te conectes a un repositorio de GitHub desde Git, deberás autenticarte con GitHub mediante HTTPS o SSH.
  * Nota: puede autenticarse en GitHub mediante el GitHub CLI, ya sea para HTTP o SSH.

<h4>Conectar con HTTPS</h4>
Si clonas con HTTPS, puedes almacenar en caché las credenciales de GitHub en Git mediante un asistente de credenciales. 

<h4>Conectar con SSH</h4>
Si clonas con SSH, debes generar claves SSH en cada equipo que uses para insertar o extraer desde GitHub. 

-------------------------------------------------------------------------------------------------------------------------------------------
<h3>Pasos siguientes</h3>
<p>Ya tienes Git y GitHub configurados. Ahora puedes elegir crear un repositorio en donde puedas poner tus proyectos. Guardar el código en un repositorio permite hacer una copia de seguridad del código y compartirlo en todo el mundo.
 
- La creación de un repositorio para el proyecto permite almacenar código en GitHub. Esto proporciona una copia de seguridad del trabajo que puedes elegir compartir con otros desarrolladores. 
- La bifurcación de un repositorio te permitirá realizar cambios en otro repositorio sin afectar al original.
- Cada repositorio de GitHub le pertenece a una persona u organización. Puedes interactuar con las personas, repositorios y organizaciones conectándote y siguiéndolos en GitHub.
- GitHub tiene una excelente comunidad de soporte técnico en la que puedes pedir ayuda y hablar con los usuarios de todo el mundo. </p>

-------------------------------------------------------------------------------------------------------------------------------------------
<h3>Configurar SSH en la Terminal</h3>

1. Buscar en la terminal con el comando which ssh-keygen, esta es la ubicación exacta de ssh-keygen.
2. Pon el comando nano ~/.zshrc_profile, te mandará a una ventana e ingresarás el comando export PATH="aqui-pon-la-ubicacion-que-buscaste-primero:$PATH".
Para guardar ese cambio con las teclas ctrl + x y te pregunta si quieres salir y guardar cambios, para guardar pulsas la tecla Y (yes); te regresa a la terminal.
3. Ingresa el comando source ~/.zshrc_profile
4. Para generar una llave escribe: ssh-keygen -t rsa -b 4096 -C "correoelectronico@gmail.com"
------------------------------------------------------------------------------------------------------------------------------------------- 
 **<p align="center">SSH-KEYGEN: es el comando para generar la llave  
 -t: significa el tipo de llave  
 rsa: es un algoritmo  
 -b: significa el tamaño en bits de la llave, en este caso es de 4096  
 -C: es comentario que se le va agregar a la llave</p>** 

-------------------------------------------------------------------------------------------------------------------------------------------
<h4>Sacar la llave a GitHub</h4>

1. Para copiar la llave, en la terminal utiliza el comando pbcopy <~/.ssh/id_rsa.pub
2. Ingresa a GitHub
3. Ingresa Settings 
4. SSH and GPG keys 
5. New SSH key
6. Ingresa un nombre 
7. Pega la llave

