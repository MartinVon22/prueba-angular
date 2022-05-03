# PruebaTecnicaAngular

Este proyecto fue generado con [Angular CLI](https://github.com/angular/angular-cli) version 13.3.3.

## Development server

Con el script `ng serve` levantamos el servidor en modo desarrollo. Navegando a `http://localhost:4200/` accedemos a la Aplicación. La aplicación cuenta con auto-realod el cual escucha cualquier cambio en algún archivo de la misma app que se haga.

## Build

Con el script `ng build` compilamos el proyecto en modo de desarrollo. Los archivos compilados son generados en el directorio `dist/`.

## ESLint

Con el script `npm run lint` comprobamos todo el código y hacemos un fix general con las reglas aplicadas en Eslint.

## Feedback

En este proyecto fue integrado ESLint y Prettier para tener un mayor órden en el código. Se usó Material Angular como motor de estructuración y diseño.

En cuanto al feedback lo que mejoraría primero es el código, hay cosas que pueden minimizarse, funciones y variables que pueden no usarse y que todo el código esté más ordenado y legible. A las funciones les agregaría comentarios para no tener que ir a cada función para ver que retorna, que parámetros espera o que hace. Luego en cuanto al Login implementaría algún tipo de storage para guardar la sesión del usuario, algun tipo de Cookie para que expire en x tiempo, para que el Login sea un poco más real. Claramente en la prueba técnica había una API para consumir y todo debía ser FrontEnd, pero yo haría un Backend para tener bien controlado que información llega a la Aplicación. Angular tiene problemas de renderización si las cosas no se hacen bien, y yo creo que la aplicación posee esos problemas, e incluso se me ha olvidado controlar variables en null o undefined, eso también lo corregiría. El diseño me ha gustado pero no el componente que he usado para el mismo ( Material Angular ), en cada componente que queremo usar pide importar el módulo en el archivo app.module. El Inicio de Sesión con Google no me ha terminado de gustar, funciona, pero podría funcionar mejor e incluso hay funciones en "deprecated" que podría corregír.

Creo que pueden haber mas cosas pero que me acuerde, por el momento son esas.

Google me pidió configurar unas Credenciales de tipo OAUTH en la consola para desarrolladores el cual tuve que hacerlo para que me de un ID y eso me dé lugar a la API para iniciar sesión con una Cuenta de Google. Actualmente el Inicio de Sesión funciona solo con mi cuenta de GMAIL, y como se configuró para modo de testeo, la cuenta de GMAIL con la que se intente loguear debo agregarla a una "lista" para darle permiso a esa cuenta que lea la API de Google usando mi cuenta como tunel. Es importante saber eso por si el inicio de sesión no funciona.
