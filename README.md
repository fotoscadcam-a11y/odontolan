## Página web de la empresa Odontolan

Este documento tendrá indicaciones sobre cómo funciona la estructura de este proyecto para futuro mantenimiento de la web.
En un principio, por como funciona hugo (el sistema usado para montar la web), la web apenas debería requerir mantenimiento, pero siempre cabe la posibilidad de que una actualización mayor cambie las cosas o que se quiera editar los contenidos de esta web.

## Estructura

NO se toca lo que hay dentro de la carpeta themes, ese es el tema que se ha usado de base para montar el resto de la web, y como base se trabaja sobre ella.
Dentro de content están los contenidos generales de la web, es decir, lo que sería el texto e información, habiendo dos subcarpetas para que la web sea multilingue.

[hugo.toml] es el archivo que tiene la configuración general de la web, aunque la mayoría de esta configuración son temas técnicos, también almacena parte de la información de la web ahí, como el nombre, favicon, etc.

Assets almacena el contenido que no sea texto, por una parte guardando las imagenes y el resto de multimedia que se utilice, y por otra las modificaciones en cuanto el aspecto de la web que aporte cambios por encima del que viene por defecto del tema. 

Layouts son contenidos que añaden modificaciones y funcionalidades a la web. En un principio no hace falta modificar nada dentro de ahí ya que son aspectos más técnicos de la web.

## Formulario

El formulario está hecho a través de Web3Forms, que es un servicio externo que hace de intermediario para mandar lo que se rellene en el formulario directamente al email enlazado.
En este momento está conectado al correo [fotoscadcam@gmail.com] en caso de que se quiera conectar a otro correo hay que crear una cuenta en su web https://web3forms.com/ e introducir la llave que se proporcione en [hugo.toml] en el parámetro [web3forms_key].