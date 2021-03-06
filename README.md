# Compilacion de aplicaciones de Javascript con Node.js 馃捇

### Este curso cuenta con 6 m贸dulos. **No se requiere requisitos previos.**
Node.js proporciona un gran conjunto de API integradas que ayudan a crear varios tipos de aplicaciones, como de l铆nea de comandos, web, etc. Tambi茅n ofrece funciones de prueba y depuraci贸n, as铆 como un amplio ecosistema de paquetes de terceros que se pueden agregar f谩cilmente a la aplicaci贸n.

## Indice: 
#### [`Modulo 1: Introducci贸n a Node.js`](#modulo-1-introducci贸n-a-node.js)
Obtenga informaci贸n sobre Node.js: qu茅 es, c贸mo funciona y cu谩ndo usarlo.


#### [`Modulo 2: Creaci贸n de un proyecto de Node.js y trabajo con dependencias`](#modulo-2-creacion-de-un-proyecto-de-Node.js-y-trabajo-con-dependencias)
Use las dependencias del registro npm para desarrollar m谩s r谩pido aplicaciones de Node.js. Obtenga informaci贸n sobre c贸mo administrar las dependencias del proyecto.

#### [`Modulo 3: Depuraci贸n interactiva de aplicaciones de Node.js con el depurador integrado y el de Visual Studio Code`](#modulo-3-depuraci贸n-interactiva-de-aplicacion-de-Node.js-con-el-depurador-integrado-y-el-de-Visual-Studio-Code)
Obtenga informaci贸n sobre c贸mo depurar de forma eficaz la aplicaci贸n de Node.js con Visual Studio Code para corregir los errores r谩pidamente.

#### [`Modulo 4:Trabajo con archivos y directorios en una aplicaci贸n Node.js`](#modulo-4-trabajo-con-archivos-y-directorios-en-una-aplicaci贸n-Node.js)
Crearemos una aplicaci贸n que manipule archivos y directorios con Node.js.


#### [`Modulo 5: Creaci贸n de una API web con Node.js y Express`](#modulo-5-creacion-de-una-api-web-con-Node.js-y-Express)
Usaremos Express para Node.js para crear API RESTful. Crearemos y configuraremos un middleware para agregar cosas como funciones de registro y de autenticaci贸n/autorizaci贸n.

#### [`Modulo 6: Introducci贸n a la administraci贸n de rutas en Node.js con JavaScript`](#modulo-6-introducci贸n-a-la-administraci贸n-de-rutas-en-Node.js-con-Javascript)
Aprenda a configurar una API de Node.js con varias rutas y a controlar las solicitudes HTTP entrantes mediante JavaScript.

<br>

# Modulo 1: Introducci贸n a Node.js 

## Indice:
#### [`Unidad 0: Introduci贸n`](#unidad-0-introducci贸n)
#### [`Unidad 1: 驴Qu茅 es Node.js`](#unidad-1-驴qu茅-es-node-js?)
#### [`Unidad 2: Funcionamineto de Node.js`](#unidad-2-funcionamiento-de-node-js)
#### [`Unidad 3: 驴Por qu茅 podr铆a necesitar Node.js?`](#unidad-3-驴por-qu茅-prodr铆a-necesitar-node-js?)
#### [`Unidad 4 Actividad en Node.js`](#unidad-4-prueba-node-js)
#### [`Unidad 5 Resumen`](#unidad-5-resumen)

<br>

# Unidad 0: Introducci贸n

## Introducci贸n
Ha sido contratado por Tailwind Traders, una gran empresa comercializadora que maneja muchos datos y archivos y tiene muchos problemas que resolver. La empresa realiza muchas operaciones mediante Node.js, pero usted no sabe c贸mo usar este entorno de tiempo de ejecuci贸n de JavaScript.
En este m贸dulo va a aprender qu茅 es Node.js y c贸mo puede usarlo para ejecutar aplicaciones y c贸digo de JavaScript fuera de un explorador. Al final de este m贸dulo podr谩 decidir si Node.js es la herramienta adecuada para el proyecto de Tailwind Traders.

## Objetivo
* Explicar qu茅 es Node.js.
* Describir c贸mo funciona Node.js.
* Identificar cu谩ndo usar Node.js.
* Crear y ejecutar un script de Node,js desde la linea de comandos. 

# Unidad 1: 驴Qu茅 es Node.js


[Node.js](https://nodejs.org/es/) (o Node para abreviar), es un entorno de ejecuci贸n de JavaScript del lado servidor de c贸digo abierto. Puede usar Node.js para ejecutar aplicaciones y c贸digo de JavaScript en muchas ubicaciones fuera de un explorador, como un servidor.
Node.js es un contenedor en torno a un motor de JavaScript denominado V8 que alimenta muchos exploradores, como Google Chrome, Opera y Microsoft Edge. Puede usar Node.js para ejecutar JavaScript mediante el motor V8 fuera de un explorador. Node.js tambi茅n contiene muchas optimizaciones de V8 que podr铆an ser necesarias para las aplicaciones que se ejecutan en un servidor. Por ejemplo, Node.js agrega una clase Buffer que permite a V8 trabajar con archivos. Esta caracter铆stica convierte a Node.js en una buena opci贸n para compilar algo como un servidor web.
Aunque nunca haya usado JavaScript como lenguaje de programaci贸n principal, podr铆a ser la opci贸n adecuada para escribir aplicaciones s贸lidas y modulares. JavaScript tambi茅n ofrece algunas ventajas exclusivas. Por ejemplo, como los exploradores usan JavaScript, puede emplear Node.js para compartir l贸gica como reglas de validaci贸n de formularios entre el explorador y el servidor.
JavaScript se ha vuelto m谩s relevante con el auge de las aplicaciones de p谩gina 煤nica y admite el formato de intercambio de datos de notaci贸n de objetos JavaScript (JSON) de uso generalizado. Muchas tecnolog铆as de base de datos NoSQL como [CouchDB](https://couchdb.apache.org/) y [MongoDB](https://www.mongodb.com/es) tambi茅n usan JavaScript y JSON como formato para consultas y esquemas. Node.js usa id茅nticos lenguaje y tecnolog铆as que muchos servicios y marcos modernos.
Con Node.js puede compilar los siguientes tipos de aplicaciones:

*	Servidores web HTTP
*	Microservicios o back-end de API sin servidor
*	Controladores para acceso a bases de datos y consulta
*	Interfaces de l铆nea de comandos interactivas
*	Aplicaciones de escritorio
*	Bibliotecas de cliente y servidor de Internet de las cosas (IoT) en tiempo real
*	Complementos para aplicaciones de escritorio
*	Scripts de shell para manipulaci贸n de archivos o acceso a la red
*	Modelos y bibliotecas de aprendizaje autom谩tico

![node](https://user-images.githubusercontent.com/80013958/168112448-e68fd674-4fb3-448c-b948-49fef0e79ccf.png)

El entorno de Node.js tambi茅n ofrece un registro [npm](https://www.npmjs.com/) que puede usar para compartir una biblioteca de Node.js propia.
Node.js es r谩pido, ofrece un alto rendimiento y puede controlar aplicaciones en tiempo real y flujos de datos intensivos. Un caso de uso de ejemplo podr铆a ser la compilaci贸n de un dispositivo que puede enviar comandos de control al escritorio permanente. Puede instalar Node.js en el panel de IoT o usar un dispositivo con Node.js preinstalado. Luego se escribir铆a la l贸gica de aplicaci贸n en JavaScript y se implementar铆a en el dispositivo.

# Unidad 2: Funcionamineto de Node.js
Como ha visto en la unidad anterior, el entorno de ejecuci贸n de JavaScript Node.js es un contenedor en torno a un motor de JavaScript denominado V8. Dado que Node.js puede interpretar y ejecutar c贸digo de JavaScript en un equipo host fuera de un explorador, el entorno de ejecuci贸n tiene acceso directo a la E/S del sistema operativo, al sistema de archivos y a la red. En esta unidad se explica c贸mo controla Node.js las tareas entrantes.

Node.js se basa en un bucle de eventos de un solo subproceso. Este modelo de arquitectura controla de forma eficaz las operaciones simult谩neas. Simultaneidad significa la capacidad del bucle de eventos de realizar funciones de devoluci贸n de llamada de JavaScript una vez completado otro trabajo.

## En este modelo de arquitectura:

* Un solo subproceso significa que JavaScript solo tiene una pila de llamadas y 煤nicamente puede realizar una operaci贸n a la vez.
* El bucle de eventos ejecuta el c贸digo, recopila y procesa eventos y ejecuta las subtareas siguientes de la cola de eventos.

Un subproceso en este contexto es una 煤nica secuencia de instrucciones programadas que el sistema operativo puede administrar de forma independiente.

En Node.js, operaciones de E/S como la lectura o escritura en un archivo en el disco o la realizaci贸n de una llamada de red a un servidor remoto se consideran operaciones de bloqueo. Una operaci贸n de bloqueo bloquea todas las tareas subsiguientes hasta que finaliza la operaci贸n, momento en que contin煤a con la siguiente operaci贸n. En un modelo sin bloqueo, el bucle de eventos puede ejecutar varias operaciones de E/S al mismo tiempo.

El nombre bucle de eventos describe el uso del mecanismo de "ocupaci贸n en espera", que espera de forma sincr贸nica a que llegue un mensaje y lo procesa. A continuaci贸n se muestra la implementaci贸n de un bucle de eventos:

    while(queue.wait()){  
         queue.proccess(); 
    }

El nombre bucle de eventos describe el uso del mecanismo de "ocupaci贸n en espera", que espera de forma sincr贸nica a que llegue un mensaje y lo procesa. A continuaci贸n se muestra la implementaci贸n de un bucle de eventos:

## Arquitectura de Node.js
Node.js usa una arquitectura controlada por eventos en la que un bucle de eventos controla la orquestaci贸n y un grupo de trabajo bloquea las tareas. El bucle de eventos permite a Node.js controlar las operaciones simult谩neas. En el siguiente diagrama se muestra c贸mo funciona un bucle de eventos, en general:

![Arquitectura de Node.js](https://docs.microsoft.com/es-mx/learn/advocates/intro-to-nodejs/media/event-loop.svg)

Las fases principales de un bucle de eventos son: 
* Los **temporizadores**: procesan las devoluciones de la llamas programadas por `setTimeout()` y `setInterval()`.
* Las **devoluciones de llamada** ejecutan devoluciones de llamadas pendientes.
* El **sondeo** recupera eventos de E/S entrantes y ejecuta devoluciones de llamadas con E/S.
* La **comprobaci贸n**: permite que las devolucuciones de llamada se ejecuten inmediantamente despu茅s de que se haya compleatado la fase de sondeo. 
* El **cierre de devoluciones de llamada** cierra eventos(por ejemplo, `socket.destroy()`) y devoluciones de llamada (por ejmplo, `socket.on('close',...)`).

Node.js usa el grupo de trabajo para controlar las tareas de bloqueo. Esto incluye las operaciones de E/S de bloqueo y las tareas con gran consumo de CPU.

En resumen, el bucle de eventos ejecuta las devoluciones de llamada de JavaScript registradas para los eventos y tambi茅n es responsable de satisfacer solicitudes asincr贸nicas sin bloqueo como la E/S de red.

## Rendimiento
JavaScript puede generar los mismos resultados de rendimiento que lenguajes de bajo nivel como C debido a las mejoras de rendimiento que posibilita el motor V8. Node.js tambi茅n aprovecha la naturaleza exclusiva controlada por eventos de JavaScript. De este modo, la creaci贸n de tareas de servidor es r谩pida y de alto rendimiento.

## Programaci贸n asincr贸nica
Para admitir el eficaz modelo de programaci贸n controlado por eventos, Node.js tiene un conjunto integrado de API de E/S sin bloqueo para controlar tareas comunes como la manipulaci贸n del sistema de archivos o de bases de datos. La biblioteca [libuv](https://libuv.org/) proporciona estas API. Al realizar una solicitud de Node.js para leer el contenido de un archivo desde un disco, Node.js no se bloquea a la espera de que el disco y los descriptores del archivo est茅n listos, sino que la interfaz de E/S sin bloqueo avisa a Node.js cuando el archivo est谩 listo. Esta E/S sin bloqueo funciona de la misma manera cuando el explorador notifica al c贸digo que se ha desencadenado un evento de mouse o teclado o cuando se ha recibido una respuesta XMLHttpRequest (XHR) desde un punto de conexi贸n remoto.

![Programacion Asincronica](https://docs.microsoft.com/es-mx/learn/advocates/intro-to-nodejs/media/architecture.svg)

## Instalaci贸n y uso de Node.js
Hay muchas formas de instalar Node.js. Estas son algunas de las opciones m谩s comunes:

* Instalaci贸n mediante un archivo ejecutable: la p谩gina Descargas de [Node.js](https://nodejs.org/en/download/) proporciona paquetes de instalaci贸n para distintos sistemas operativos.
* Instalaci贸n mediante Brew: Brew es un conocido administrador de paquetes para Linux y macOS.
* Instalaci贸n mediante NVM: Node Version Manager (NVM) no solo ayuda a instalar la versi贸n de Node.js que se quiera, sino tambi茅n a administrar la instalaci贸n. Esta opci贸n no se trata en esta secci贸n.

Vamos a echar un vistazo m谩s detallado a los pasos necesarios para descargar e instalar Node.js y comprobar la correcci贸n de la instalaci贸n.

## Instalaci贸n mediante un archivo ejecutable

![install-page](https://user-images.githubusercontent.com/80013958/168113442-c5d5e97f-d4cc-4f35-943f-431fe33e24c6.png)


Observe los distintos instaladores disponibles para diferentes sistemas operativos como Windows, macOS y Linux. Tambi茅n puede descargar dos versiones de c贸digo fuente diferentes:

* **LTS** significa Long-Term-Support (soporte tecnico a largo plazo). Tenga en cuenta que LTS se describe como **Recomendado para la mayoria de usuarios**. LTS est谩 dise帽ado para el uso empresarial en el que es posible que las actualizaciones frecuentes no sean posibles ni deseadas.

* **Actual** significa c贸digo fuente que est谩 en desarrollo activo. Es posible que se produzcan adiciones de caracter铆sticas y cambios importantes. El c贸digo se debe adherir al control de versiones sem谩ntico.

Base la elecci贸n de versi贸n en los requisitos de la empresa. Por ejemplo, si actualiza con frecuencia, la versi贸n Actual puede ser la adecuada.

## Instalaci贸n mediante el administrador de paquetes Brew
Si no tiene instalado Brew, ejecute este comando en el terminal de macOS o Linux:

    /bin/bash - c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
Despu茅s de descargar Brew, escriba el siguiente comando en el terminal para iniciar la instalaci贸n:

    brew install node
Esto descarga todos los archivos binarios necesarios e instala Node.js en el sistema.

## Comprobaci贸n de la instalaci贸n
Una vez finalizada la instalaci贸n de Node.js, ejecute el siguiente comando en el terminal para comprobar que la instalaci贸n se ha realizado correctamente:

    node --version
El comando debe imprimir la versi贸n actual en el formato siguiente:

    v[major version].[minor version].[patch version]



# Unidad 3: 驴Por qu茅 podr铆a necesitar Node.js

## 驴Por qu茅 podr铆a necesitar Node.js?

Node.js es una de las tecnolog铆as de uso m谩s generalizado en compa帽铆as, startups y organizaciones gubernamentales. Entre ellas se incluyen importantes empresas como Netflix, Trello, Walmart, Uber, eBay y NASA.

Node.js es un entorno de ejecuci贸n de JavaScript que puede ejecutar aplicaciones y c贸digo de JavaScript en un servidor en concreto, y fuera de un explorador en general. Node.js es un entorno de tiempo de ejecuci贸n sin bloqueo de un solo subproceso que se basa en el paradigma de E/S controlado por eventos. Sin bloqueo significa que, por ejemplo, si un cliente remoto realiza una solicitud, un servidor escrito en JavaScript y que se ejecuta en Node.js controla la solicitud, elabora y devuelve una respuesta y luego pasa a la solicitud siguiente, sin bloquear ni esperar a que finalicen otras tareas.

En esta unidad se describen las ventajas principales del uso de Node.js y cu谩ndo usarlo.

## Tecnolog铆a multiuso

Puede usar Node.js para compilar una amplia variedad de aplicaciones listas para producci贸n. Estas abarcan desde aplicaciones tradicionales ligeras de chat con tr谩fico elevado a herramientas de l铆nea de comandos y servidores web. Node.js se ha dise帽ado desde cero para controlar un gran n煤mero de solicitudes simult谩neas.

## JavaScript

"Toda aplicaci贸n que se pueda escribir en JavaScript, se escribir谩 finalmente en JavaScript". 鈥? Jeff Atwood, escritor, empresario, cofundador de StackOverflow.

Hoy en d铆a, muchas aplicaciones escritas fuera del explorador est谩n en JavaScript o admiten este lenguaje como ciudadano de primera clase, incluidas:

* Editores de c贸digo como Visual Studio Code y Atom, que est谩n escritos en JavaScript o TypeScript (un superconjunto de JavaScript con tipos est谩ticos). Estos editores ejecutan una versi贸n insertada del entorno de ejecuci贸n Node.js.
* Muchas aplicaciones de Internet de las cosas (IoT) y en tiempo real que est谩n escritas en JavaScript y dependen de Node.js para ejecutarse, ya sea en el servidor o a trav茅s de microcontroladores y plataformas SoC (Sistema en un chip), como Puck.js o Tessel.
* Tecnolog铆as como NativeScript que pueden usar JavaScript o TypeScript para compilar aplicaciones para dispositivos m贸viles nativas de alto rendimiento.
* Muchas aplicaciones que usan JavaScript para su sistema de complementos, como Sketch, Adobe XD y Google Apps Script.

## Comunidad

La comunidad ya ha compilado m谩s de un mill贸n de m贸dulos y bibliotecas para Node.js y las ha publicado en el administrador de paquetes de Node (NPM). Los desarrolladores pueden descargar e integrar f谩cilmente esos m贸dulos en los proyectos existentes. Las aplicaciones que se pueden ejecutar en Node.js incluyen herramientas de l铆nea de comandos, marcos, servidores web, etc.

## C贸digo abierto

Node.js es una tecnolog铆a de c贸digo abierto admitida por OpenJS Foundation. Cuenta con una numerosa y activa comunidad de c贸digo abierto y colaboradores que trabajan sin descanso para mejorar y optimizar la tecnolog铆a. Un comit茅 de la comunidad de alto nivel tiene autoridad sobre los esfuerzos de promoci贸n de la comunidad.

# Unidad 4 Actividad en Node.js
En esta unidad va a crear y ejecutar un sencillo script de Node.js Hola mundo.

## REPL de Node.js
Node.js tiene un modo **read-eval-print loop** (REPL) integrado que resulta 煤til para la evaluaci贸n r谩pida de c贸digo y la experimentaci贸n. El modo REPL es un entorno de consola interactivo en el que se puede escribir c贸digo de JavaScript para que Node.js lo interprete y lo ejecute y luego imprima el resultado.

El modo REPL de Node.js funciona de la siguiente manera:

* **Lectura**: lee y analiza la entrada de c贸digo de JavaScript del usuario (o  muestra un error si el c贸digo no es v谩lido).
* **Evaluaci贸n**: eval煤a el c贸digo de JavaScript especificado.
* **Impresi贸n**: imprime los resultados calculados.
* **Bucle**: itera en bucle y espera a que el usuario escriba un comando nuevo (o sale si el usuario presiona **Ctrl-C** dos veces).

Para iniciar el modo REPL, ejecute el programa node en la consola de su sistema operativo: 

`bash`

    node
Se abre el entorno de REPL. Deber铆a ver el siguiente resultado:

`text`

    >
Intente escribir el c贸digo **console.log('Hello World, from the REPL.')** dentro de la consola de REPL y vea el resultado. Este c贸digo imprime un mensaje "Hola mundo, desde REPL." en la salida de REPL:

`text`

    > console.log('Hello World, from the REPL.')
    Hello Worldm from the REPL
Para salir del entorno de REPL, presione Ctrl-C dos veces:

`text`

    >
    (To exit, press ^C again or type .exit)
    >

## Creaci贸n de un script de Node.js

Node.js tambi茅n asdmite la ejecucion de c贸digo desde archivos

* 1- Desde la consola del sistema operativo, escriba el comando **code** para abrir un nuevo editor:

    `bash`

        code
* 2- Dentro del editor de c贸digo deber谩 crear un archivo con la extenci贸n **.js** (puede tener cualquier nombre pero por lo general se llama app.js o index.js) en la que le va a colocar el siguiente codigo:

    `Javascript`
    
        console.log('Hello World, from script file.');
* 3- Guarde el archivo al presionar **Ctrl+s** (Windows, Linux) o **Cmd+s** (macOS) en index.js

* 4- En su consola de linea de comandos, escriba **node** seguido por el nombre del archivo con la extensi贸n **.js**, en este caso index.js

    `Javascript`
        
        node index.js

Deber铆a ver el siguiente resultado:

`text`

    $ node index.js
    Hello World, from a script file.

Ya ha ejecutado el primer c贸digo propio de JavaScript Node.js.

# Unidad 5 Resumen

## Resumen
En este m贸dulo ha aprendido que Node.js es un entorno de ejecuci贸n que puede ejecutar aplicaciones y c贸digo de JavaScript fuera de un explorador. Tambi茅n ha aprendido c贸mo funciona Node.js y por qu茅 es una buena opci贸n para compilar y ejecutar aplicaciones de JavaScript. Esto puede abarcar desde la compilaci贸n de servidores de aplicaciones hasta la ejecuci贸n de aplicaciones en tiempo real en dispositivos insertados de Internet de las cosas (IoT).

## Recursos adicionales
Las siguientes aplicaciones se compilan con Node.js:

* Herramientas de la CLI, como: [hexa.run](https://hexa.run/) y [CLI de Azure Fundations](https://github.com/Azure/azure-functions-core-tools)

* Servidores de Back-End y de servicios API como [Express.js](https://expressjs.com/) y [Nest.js](https://nestjs.com/)

* Aplicaciones de escritorios, como [Slack](https://slack.com/intl/es-ar/) con [Electron](https://www.electronjs.org/)

* Bibliotecas de IoT, como [Johnny-Five](https://johnny-five.io/), [Puck-js](https://www.puck-js.com/) y [Tessel](https://tessel.io/)

* Complementos para [SketchApp](https://www.sketch.com/) y [Adobe XD](https://www.adobe.com/products/xd.html)

* Editores de c贸digo, como [Visual Studio Code](https://code.visualstudio.com/) y [Atom](https://atom.io/)

* Desarrollo para dispositivos m贸viles nativo con [NativeScript](https://nativescript.org/)

Las t茅cnicas de optimizaci贸n de compilaci贸n incluyen:

* [JIT](https://en.wikipedia.org/wiki/Just-in-time_compilation)
* [Optimizaci贸n especulativa simult谩nea](https://ponyfoo.com/articles/an-introduction-to-speculative-optimization-in-v8)

Las empresas que usan Node.js en producci贸n incluyen:
* [Netflix](https://www.youtube.com/watch?v=p74282nDMX8)
* [Trello](https://tech.trello.com/the-trello-tech-stack/)
* [Wallmart](https://medium.com/walmartglobaltech/migrating-large-enterprise-to-nodejs-6c38523d2b33)
* [Uber](https://eng.uber.com/uber-tech-stack-part-two/)
* [eBay](https://eng.uber.com/uber-tech-stack-part-two/)
* [NASA](https://openjsf.org/wp-content/uploads/sites/84/2020/02/Case_Study-Node.js-NASA.pdf)

Tipos de versi贸n de Node.js:
* [Tipos de Versi贸n](https://github.com/nodejs/node#release-types)
