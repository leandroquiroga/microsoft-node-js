# Compilacion de aplicaciones de Javascript con Node.js 💻

### Este curso cuenta con 6 módulos. **No se requiere requisitos previos.**
Node.js proporciona un gran conjunto de API integradas que ayudan a crear varios tipos de aplicaciones, como de línea de comandos, web, etc. También ofrece funciones de prueba y depuración, así como un amplio ecosistema de paquetes de terceros que se pueden agregar fácilmente a la aplicación.

## Indice: 
#### [`Modulo 1: Introducción a Node.js `](#modulo-1-introducción-a-node.js)
Obtenga información sobre Node.js: qué es, cómo funciona y cuándo usarlo.


#### [`Modulo 2: Creación de un proyecto de Node.js y trabajo con dependencias`](#modulo-2-creacion-de-un-proyecto-de-node.js-y-trabajo-con-dependencias)
Use las dependencias del registro npm para desarrollar más rápido aplicaciones de Node.js. Obtenga información sobre cómo administrar las dependencias del proyecto.

#### [`Modulo 3: Depuración interactiva de aplicaciones de Node.js con el depurador integrado y el de Visual Studio Code`](#modulo-3-depuración-interactiva-de-aplicacion-de-node.js-con-el-depurador-integrado-y-el-de-visual-studio-code)
Obtenga información sobre cómo depurar de forma eficaz la aplicación de Node.js con Visual Studio Code para corregir los errores rápidamente.

#### [`Modulo 4:Trabajo con archivos y directorios en una aplicación Node.js`](#modulo-4-trabajo-con-archivos-y-directorios-en-una-aplicación-node.js)
Crearemos una aplicación que manipule archivos y directorios con Node.js.


#### [`Modulo 5: Creación de una API web con Node.js y Express`](#modulo-5-creacion-de-una-api-web-con-node.js-y-express)
Usaremos Express para Node.js para crear API RESTful. Crearemos y configuraremos un middleware para agregar cosas como funciones de registro y de autenticación/autorización.

#### [`Modulo 6: Introducción a la administración de rutas en Node.js con JavaScript`](#modulo-6-introducción-a-la-administración-de-rutas-en-node.js-con-javascript)
Aprenda a configurar una API de Node.js con varias rutas y a controlar las solicitudes HTTP entrantes mediante JavaScript.

<br>

# Modulo 1: Introducción a Node.js 

## Indice:
#### [`Unidad 0: Introdución`](#unidad-0-introducción)
#### [`Unidad 1: ¿Qué es Node.js`](#unidad-1-¿qué-es-node-js?)
#### [`Unidad 2: Funcionamineto de Node.js`](#unidad-2-funcionamiento-de-node-js)
#### [`Unidad 3: ¿Por qué podría necesitar Node.js?`](#unidad-3-¿por-qué-prodría-necesitar-node-js?)
#### [`Unidad 4 Actividad en Node.js`](#unidad-4-prueba-node-js)
#### [`Unidad 5 Resumen`](#unidad-5-resumen)

<br>

# Unidad 0: Introducción

## Introducción
Ha sido contratado por Tailwind Traders, una gran empresa comercializadora que maneja muchos datos y archivos y tiene muchos problemas que resolver. La empresa realiza muchas operaciones mediante Node.js, pero usted no sabe cómo usar este entorno de tiempo de ejecución de JavaScript.
En este módulo va a aprender qué es Node.js y cómo puede usarlo para ejecutar aplicaciones y código de JavaScript fuera de un explorador. Al final de este módulo podrá decidir si Node.js es la herramienta adecuada para el proyecto de Tailwind Traders.

## Objetivo
* Explicar qué es Node.js.
* Describir cómo funciona Node.js.
* Identificar cuándo usar Node.js.
* Crear y ejecutar un script de Node,js desde la linea de comandos. 

# Unidad 1: ¿Qué es Node.js


[Node.js](https://nodejs.org/es/) (o Node para abreviar), es un entorno de ejecución de JavaScript del lado servidor de código abierto. Puede usar Node.js para ejecutar aplicaciones y código de JavaScript en muchas ubicaciones fuera de un explorador, como un servidor.
Node.js es un contenedor en torno a un motor de JavaScript denominado V8 que alimenta muchos exploradores, como Google Chrome, Opera y Microsoft Edge. Puede usar Node.js para ejecutar JavaScript mediante el motor V8 fuera de un explorador. Node.js también contiene muchas optimizaciones de V8 que podrían ser necesarias para las aplicaciones que se ejecutan en un servidor. Por ejemplo, Node.js agrega una clase Buffer que permite a V8 trabajar con archivos. Esta característica convierte a Node.js en una buena opción para compilar algo como un servidor web.
Aunque nunca haya usado JavaScript como lenguaje de programación principal, podría ser la opción adecuada para escribir aplicaciones sólidas y modulares. JavaScript también ofrece algunas ventajas exclusivas. Por ejemplo, como los exploradores usan JavaScript, puede emplear Node.js para compartir lógica como reglas de validación de formularios entre el explorador y el servidor.
JavaScript se ha vuelto más relevante con el auge de las aplicaciones de página única y admite el formato de intercambio de datos de notación de objetos JavaScript (JSON) de uso generalizado. Muchas tecnologías de base de datos NoSQL como [CouchDB](https://couchdb.apache.org/) y [MongoDB](https://www.mongodb.com/es) también usan JavaScript y JSON como formato para consultas y esquemas. Node.js usa idénticos lenguaje y tecnologías que muchos servicios y marcos modernos.
Con Node.js puede compilar los siguientes tipos de aplicaciones:
´
*	Servidores web HTTP
*	Microservicios o back-end de API sin servidor
*	Controladores para acceso a bases de datos y consulta
*	Interfaces de línea de comandos interactivas
*	Aplicaciones de escritorio
*	Bibliotecas de cliente y servidor de Internet de las cosas (IoT) en tiempo real
*	Complementos para aplicaciones de escritorio
*	Scripts de shell para manipulación de archivos o acceso a la red
*	Modelos y bibliotecas de aprendizaje automático

El entorno de Node.js también ofrece un registro [npm](https://www.npmjs.com/) que puede usar para compartir una biblioteca de Node.js propia.
Node.js es rápido, ofrece un alto rendimiento y puede controlar aplicaciones en tiempo real y flujos de datos intensivos. Un caso de uso de ejemplo podría ser la compilación de un dispositivo que puede enviar comandos de control al escritorio permanente. Puede instalar Node.js en el panel de IoT o usar un dispositivo con Node.js preinstalado. Luego se escribiría la lógica de aplicación en JavaScript y se implementaría en el dispositivo.

# Unidad 2: Funcionamineto de Node.js
Como ha visto en la unidad anterior, el entorno de ejecución de JavaScript Node.js es un contenedor en torno a un motor de JavaScript denominado V8. Dado que Node.js puede interpretar y ejecutar código de JavaScript en un equipo host fuera de un explorador, el entorno de ejecución tiene acceso directo a la E/S del sistema operativo, al sistema de archivos y a la red. En esta unidad se explica cómo controla Node.js las tareas entrantes.

Node.js se basa en un bucle de eventos de un solo subproceso. Este modelo de arquitectura controla de forma eficaz las operaciones simultáneas. Simultaneidad significa la capacidad del bucle de eventos de realizar funciones de devolución de llamada de JavaScript una vez completado otro trabajo.

## En este modelo de arquitectura:

* Un solo subproceso significa que JavaScript solo tiene una pila de llamadas y únicamente puede realizar una operación a la vez.
* El bucle de eventos ejecuta el código, recopila y procesa eventos y ejecuta las subtareas siguientes de la cola de eventos.

Un subproceso en este contexto es una única secuencia de instrucciones programadas que el sistema operativo puede administrar de forma independiente.

En Node.js, operaciones de E/S como la lectura o escritura en un archivo en el disco o la realización de una llamada de red a un servidor remoto se consideran operaciones de bloqueo. Una operación de bloqueo bloquea todas las tareas subsiguientes hasta que finaliza la operación, momento en que continúa con la siguiente operación. En un modelo sin bloqueo, el bucle de eventos puede ejecutar varias operaciones de E/S al mismo tiempo.

El nombre bucle de eventos describe el uso del mecanismo de "ocupación en espera", que espera de forma sincrónica a que llegue un mensaje y lo procesa. A continuación se muestra la implementación de un bucle de eventos:

    while(queue.wait()){  
         queue.proccess(); 
    }

El nombre bucle de eventos describe el uso del mecanismo de "ocupación en espera", que espera de forma sincrónica a que llegue un mensaje y lo procesa. A continuación se muestra la implementación de un bucle de eventos:

## Arquitectura de Node.js
Node.js usa una arquitectura controlada por eventos en la que un bucle de eventos controla la orquestación y un grupo de trabajo bloquea las tareas. El bucle de eventos permite a Node.js controlar las operaciones simultáneas. En el siguiente diagrama se muestra cómo funciona un bucle de eventos, en general:

(*Insertar imagen de la arquitectura de node*)

Las fases principales de un bucle de eventos son: 
* Los **temporizadores**: procesan las devoluciones de la llamas programadas por `setTimeout()` y `setInterval()`.
* Las **devoluciones de llamada** ejecutan devoluciones de llamadas pendientes.
* El **sondeo** recupera eventos de E/S entrantes y ejecuta devoluciones de llamadas con E/S.
* La **comprobación**: permite que las devolucuciones de llamada se ejecuten inmediantamente después de que se haya compleatado la fase de sondeo. 
* El **cierre de devoluciones de llamada** cierra eventos(por ejemplo, `socket.destroy()`) y devoluciones de llamada (por ejmplo, `socket.on('close',...)`).

Node.js usa el grupo de trabajo para controlar las tareas de bloqueo. Esto incluye las operaciones de E/S de bloqueo y las tareas con gran consumo de CPU.

En resumen, el bucle de eventos ejecuta las devoluciones de llamada de JavaScript registradas para los eventos y también es responsable de satisfacer solicitudes asincrónicas sin bloqueo como la E/S de red.

## Rendimiento
JavaScript puede generar los mismos resultados de rendimiento que lenguajes de bajo nivel como C debido a las mejoras de rendimiento que posibilita el motor V8. Node.js también aprovecha la naturaleza exclusiva controlada por eventos de JavaScript. De este modo, la creación de tareas de servidor es rápida y de alto rendimiento.

## Programación asincrónica
Para admitir el eficaz modelo de programación controlado por eventos, Node.js tiene un conjunto integrado de API de E/S sin bloqueo para controlar tareas comunes como la manipulación del sistema de archivos o de bases de datos. La biblioteca [libuv](https://libuv.org/) proporciona estas API. Al realizar una solicitud de Node.js para leer el contenido de un archivo desde un disco, Node.js no se bloquea a la espera de que el disco y los descriptores del archivo estén listos, sino que la interfaz de E/S sin bloqueo avisa a Node.js cuando el archivo está listo. Esta E/S sin bloqueo funciona de la misma manera cuando el explorador notifica al código que se ha desencadenado un evento de mouse o teclado o cuando se ha recibido una respuesta XMLHttpRequest (XHR) desde un punto de conexión remoto.

(*Insertar imagen de la programacion asincronica*);

## Instalación y uso de Node.js
Hay muchas formas de instalar Node.js. Estas son algunas de las opciones más comunes:

* Instalación mediante un archivo ejecutable: la página Descargas de [Node.js](https://nodejs.org/en/download/) proporciona paquetes de instalación para distintos sistemas operativos.
* Instalación mediante Brew: Brew es un conocido administrador de paquetes para Linux y macOS.
* Instalación mediante NVM: Node Version Manager (NVM) no solo ayuda a instalar la versión de Node.js que se quiera, sino también a administrar la instalación. Esta opción no se trata en esta sección.

Vamos a echar un vistazo más detallado a los pasos necesarios para descargar e instalar Node.js y comprobar la corrección de la instalación.

## Instalación mediante un archivo ejecutable

(*Insertar imagen de la descarga de node.js*);

Observe los distintos instaladores disponibles para diferentes sistemas operativos como Windows, macOS y Linux. También puede descargar dos versiones de código fuente diferentes:

* **LTS** significa Long-Term-Support (soporte tecnico a largo plazo). Tenga en cuenta que LTS se describe como **Recomendado para la mayoria de usuarios**. LTS está diseñado para el uso empresarial en el que es posible que las actualizaciones frecuentes no sean posibles ni deseadas.

* **Actual** significa código fuente que está en desarrollo activo. Es posible que se produzcan adiciones de características y cambios importantes. El código se debe adherir al control de versiones semántico.

Base la elección de versión en los requisitos de la empresa. Por ejemplo, si actualiza con frecuencia, la versión Actual puede ser la adecuada.

## Instalación mediante el administrador de paquetes Brew
Si no tiene instalado Brew, ejecute este comando en el terminal de macOS o Linux:

    /bin/bash - c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
Después de descargar Brew, escriba el siguiente comando en el terminal para iniciar la instalación:

    brew install node
Esto descarga todos los archivos binarios necesarios e instala Node.js en el sistema.

## Comprobación de la instalación
Una vez finalizada la instalación de Node.js, ejecute el siguiente comando en el terminal para comprobar que la instalación se ha realizado correctamente:

    node --version
El comando debe imprimir la versión actual en el formato siguiente:

    v[major version].[minor version].[patch version]



# Unidad 3: ¿Por qué podría necesitar Node.js

## ¿Por qué podría necesitar Node.js?

Node.js es una de las tecnologías de uso más generalizado en compañías, startups y organizaciones gubernamentales. Entre ellas se incluyen importantes empresas como Netflix, Trello, Walmart, Uber, eBay y NASA.

Node.js es un entorno de ejecución de JavaScript que puede ejecutar aplicaciones y código de JavaScript en un servidor en concreto, y fuera de un explorador en general. Node.js es un entorno de tiempo de ejecución sin bloqueo de un solo subproceso que se basa en el paradigma de E/S controlado por eventos. Sin bloqueo significa que, por ejemplo, si un cliente remoto realiza una solicitud, un servidor escrito en JavaScript y que se ejecuta en Node.js controla la solicitud, elabora y devuelve una respuesta y luego pasa a la solicitud siguiente, sin bloquear ni esperar a que finalicen otras tareas.

En esta unidad se describen las ventajas principales del uso de Node.js y cuándo usarlo.

## Tecnología multiuso

Puede usar Node.js para compilar una amplia variedad de aplicaciones listas para producción. Estas abarcan desde aplicaciones tradicionales ligeras de chat con tráfico elevado a herramientas de línea de comandos y servidores web. Node.js se ha diseñado desde cero para controlar un gran número de solicitudes simultáneas.

## JavaScript

"Toda aplicación que se pueda escribir en JavaScript, se escribirá finalmente en JavaScript". – Jeff Atwood, escritor, empresario, cofundador de StackOverflow.

Hoy en día, muchas aplicaciones escritas fuera del explorador están en JavaScript o admiten este lenguaje como ciudadano de primera clase, incluidas:

* Editores de código como Visual Studio Code y Atom, que están escritos en JavaScript o TypeScript (un superconjunto de JavaScript con tipos estáticos). Estos editores ejecutan una versión insertada del entorno de ejecución Node.js.
* Muchas aplicaciones de Internet de las cosas (IoT) y en tiempo real que están escritas en JavaScript y dependen de Node.js para ejecutarse, ya sea en el servidor o a través de microcontroladores y plataformas SoC (Sistema en un chip), como Puck.js o Tessel.
* Tecnologías como NativeScript que pueden usar JavaScript o TypeScript para compilar aplicaciones para dispositivos móviles nativas de alto rendimiento.
* Muchas aplicaciones que usan JavaScript para su sistema de complementos, como Sketch, Adobe XD y Google Apps Script.

## Comunidad

La comunidad ya ha compilado más de un millón de módulos y bibliotecas para Node.js y las ha publicado en el administrador de paquetes de Node (NPM). Los desarrolladores pueden descargar e integrar fácilmente esos módulos en los proyectos existentes. Las aplicaciones que se pueden ejecutar en Node.js incluyen herramientas de línea de comandos, marcos, servidores web, etc.

## Código abierto

Node.js es una tecnología de código abierto admitida por OpenJS Foundation. Cuenta con una numerosa y activa comunidad de código abierto y colaboradores que trabajan sin descanso para mejorar y optimizar la tecnología. Un comité de la comunidad de alto nivel tiene autoridad sobre los esfuerzos de promoción de la comunidad.

# Unidad 4 Actividad en Node.js
En esta unidad va a crear y ejecutar un sencillo script de Node.js Hola mundo.

## REPL de Node.js
Node.js tiene un modo **read-eval-print loop** (REPL) integrado que resulta útil para la evaluación rápida de código y la experimentación. El modo REPL es un entorno de consola interactivo en el que se puede escribir código de JavaScript para que Node.js lo interprete y lo ejecute y luego imprima el resultado.

El modo REPL de Node.js funciona de la siguiente manera:

* **Lectura**: lee y analiza la entrada de código de JavaScript del usuario (o  muestra un error si el código no es válido).
* **Evaluación**: evalúa el código de JavaScript especificado.
* **Impresión**: imprime los resultados calculados.
* **Bucle**: itera en bucle y espera a que el usuario escriba un comando nuevo (o sale si el usuario presiona **Ctrl-C** dos veces).

Para iniciar el modo REPL, ejecute el programa node en la consola de su sistema operativo: 

`bash`

    node
Se abre el entorno de REPL. Debería ver el siguiente resultado:

`text`

    >
Intente escribir el código **console.log('Hello World, from the REPL.')** dentro de la consola de REPL y vea el resultado. Este código imprime un mensaje "Hola mundo, desde REPL." en la salida de REPL:

`text`

    > console.log('Hello World, from the REPL.')
    Hello Worldm from the REPL
Para salir del entorno de REPL, presione Ctrl-C dos veces:

`text`

    >
    (To exit, press ^C again or type .exit)
    >

## Creación de un script de Node.js

Node.js también asdmite la ejecucion de código desde archivos

* 1- Desde la consola del sistema operativo, escriba el comando **code** para abrir un nuevo editor:

    `bash`

        code
* 2- Dentro del editor de código deberá crear un archivo con la extención **.js** (puede tener cualquier nombre pero por lo general se llama app.js o index.js) en la que le va a colocar el siguiente codigo:

    `Javascript`
    
        console.log('Hello World, from script file.');
* 3- Guarde el archivo al presionar **Ctrl+s** (Windows, Linux) o **Cmd+s** (macOS) en index.js

* 4- En su consola de linea de comandos, escriba **node** seguido por el nombre del archivo con la extensión **.js**, en este caso index.js

    `Javascript`
        
        node index.js

Debería ver el siguiente resultado:

`text`

    $ node index.js
    Hello World, from a script file.

Ya ha ejecutado el primer código propio de JavaScript Node.js.

# Unidad 5 Resumen

## Resumen
En este módulo ha aprendido que Node.js es un entorno de ejecución que puede ejecutar aplicaciones y código de JavaScript fuera de un explorador. También ha aprendido cómo funciona Node.js y por qué es una buena opción para compilar y ejecutar aplicaciones de JavaScript. Esto puede abarcar desde la compilación de servidores de aplicaciones hasta la ejecución de aplicaciones en tiempo real en dispositivos insertados de Internet de las cosas (IoT).

## Recursos adicionales
Las siguientes aplicaciones se compilan con Node.js:

* Herramientas de la CLI, como: [hexa.run](https://hexa.run/) y [CLI de Azure Fundations](https://github.com/Azure/azure-functions-core-tools)

* Servidores de Back-End y de servicios API como [Express.js](https://expressjs.com/) y [Nest.js](https://nestjs.com/)

* Aplicaciones de escritorios, como [Slack](https://slack.com/intl/es-ar/) con [Electron](https://www.electronjs.org/)

* Bibliotecas de IoT, como [Johnny-Five](https://johnny-five.io/), [Puck-js](https://www.puck-js.com/) y [Tessel](https://tessel.io/)

* Complementos para [SketchApp](https://www.sketch.com/) y [Adobe XD](https://www.adobe.com/products/xd.html)

* Editores de código, como [Visual Studio Code](https://code.visualstudio.com/) y [Atom](https://atom.io/)

* Desarrollo para dispositivos móviles nativo con [NativeScript](https://nativescript.org/)

Las técnicas de optimización de compilación incluyen:

* [JIT](https://en.wikipedia.org/wiki/Just-in-time_compilation)
* [Optimización especulativa simultánea](https://ponyfoo.com/articles/an-introduction-to-speculative-optimization-in-v8)

Las empresas que usan Node.js en producción incluyen:
* [Netflix](https://www.youtube.com/watch?v=p74282nDMX8)
* [Trello](https://tech.trello.com/the-trello-tech-stack/)
* [Wallmart](https://medium.com/walmartglobaltech/migrating-large-enterprise-to-nodejs-6c38523d2b33)
* [Uber](https://eng.uber.com/uber-tech-stack-part-two/)
* [eBay](https://eng.uber.com/uber-tech-stack-part-two/)
* [NASA](https://openjsf.org/wp-content/uploads/sites/84/2020/02/Case_Study-Node.js-NASA.pdf)

Tipos de versión de Node.js:
* [Tipos de Versión](https://github.com/nodejs/node#release-types)
