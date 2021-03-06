# Visual Studio Code

## 1. Que es Visual Studio Code?

Visual Studio Code es un editor de código fuente desarrollado por Microsoft para Windows , Linux y macOS. Incluye soporte para la depuración, control integrado de Git, resaltado de sintaxis, finalización inteligente de código, fragmentos y refactorización de código. También es personalizable, por lo que los usuarios pueden cambiar el tema del editor, los atajos de teclado y las preferencias. Es gratuito y de código abierto, aunque la descarga oficial está bajo software propietario requiriendo tus datos de uso del programa legalmente.

Visual Studio Code se basa en Electron, un framework que se utiliza para implementar aplicaciones Node.js para el escritorio, que se ejecuta en el motor de diseño Blink. Aunque utiliza el framework Electron, el software no usa Atom y en su lugar emplea el mismo componente editor (Monaco) utilizado en Visual Studio Team Services (anteriormente llamado Visual Studio Online).

## 2. Como se instalan extensiones?

Para instalar extensiones en VSCode, es muy sencillo, simplemente, en la barra de la izquierda, clickaremos sobre la ultima opción, como podemos ver ne la imagen a continuación:

![extensionesVSCode](https://github.com/enriquepoler/EDD/blob/master/img/captura1VSCode.png)

El siguiente paso será buscar en la barra de busqueda, la extensión que queramos instalar, y le daremos a instalar sobre el boton verde, podemos verlo en la imagen a continuación:

![InstalaExtensionesVSCode](https://github.com/enriquepoler/EDD/blob/master/img/captura2VSCode.png)

Y si esta extensión necesita otras extensiones para funcionar, se pondran a instalarse todas a la vez como podemos ver en la siguiente imagen:

![InstalandoExtensionesVSCode](https://github.com/enriquepoler/EDD/blob/master/img/captura3VSCode.png)

Una vez esté instalado todo, deberemos acceder al archivo de configuración del java.home o JDK, podemos hacerlo a traves de la pestaña del VSCode, Archivo, Preferencias, Configuración. Una vez llegados a este punto, en la barra de búsqueda de configuración, podemos poner o java.home o jdk, y entramos en el archivo de configuración de la primera busqueda. una vez en el archivo, añadiremos una nueva linea, primero pondremos una "," en el final de la ultima linea, para separar, y en la linea siguiente escribiremos "java.json": "ruta_del_openjdk". En la siguiente imagen tenemos un ejemplo, en mi caso la ruta es "/usr/lib/jvm/java-11-openjdk-amd64":

![AgregarOpenJDK](https://github.com/enriquepoler/EDD/blob/master/img/captura4VSCode.png)
