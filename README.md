# Vue App para generar contraseñas con dos metodos

Web app realizada con Vue y Vite para la creación de contraseñas con diferentes caracteres.

## Proximamente

- Actualizaciones anteriormente dichas
- Mejora en la interfaz completa
- Menú principal para utilizar las SPA nativas de Vue

## Incluye

Dos métodos para crear contraseñas
Caracteres incluidos:

abcdefghijklmnopqrstuvwxyz

ABCDEFGHIJKLMNOPQRSTUVWXYZ

0123456789

![]{}()%&*$#^<>~@|

## Instalación

```
git clone https://github.com/smartinez05/vue-password-generator.git
cd vue-password-generator
npm install
npm run dev
```
Ir a http://localhost:3000

## Metodo 1 - Password.vue

*Basado en el [Codepen de Christophor Wilson](https://codepen.io/CSWApps/pen/QvYNMM). Créditos al autor.*

Por cada toque en el botón Generar contraseña se generará una nueva con los mismos caracteres. En el momento solo crea contraseñas de 10 carácteres.

*En una próxima actualización se añadirán más opciones para hacer contraseñas*

## Método 2 - Password2.Vue

*Basado en el [video de Webnoob/Mario Laurich](https://www.youtube.com/watch?v=6ZnnrgmDlkM). Créditos al autor.*

- Utiliza crypto para generar contraseñas mas seguras.
- Se puede escoger el tamaño de la contraseña, iniciando desde 16.
- Se puede escoger los caracteres deseados en la contraseña.

*En una próxima actualización revisaré las funciones detalladamente y mejoraré el estilo del cajón.*

