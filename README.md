# WEBPACK
 webpack solamente entiende JavaScript y JSON. Los loaders nos permite procesar archivos de otros tipos para convertirnos en módulos válidos que serán consumidos por nuestras aplicaciones y agregadas como dependencias.

En alto nivel, los loaders poseen 2 configuraciones principales:

test - propiedad que identifica cuáles archivos deberán ser transformados
use - propiedad que identifica el loader que será usado para transformar a dichos archivos

Plugins
Mientras los loaders transforman ciertos tipos de módulos, los plugins son utilizados para extender tareas específicas, como la optimización de paquetes, la gestión de activos y la inyección de variables de entorno.

Una vez importado el plugin, podemos desear el personalizarlos a través de opciones.

## Babel Loader (Javascript)
Babel te permite hacer que tu código JavaScript sea compatible con todos los navegadores
Debes agregar a tu proyecto las siguientes dependencias

```bash
npm install -D babel-loader @babel/core @babel/preset-env @babel/preset-react @babel/plugin-transform-runtime babel-eslint
```

## Htm en Webpack
Es un plugin para inyectar javascript, css, favicons, y nos facilita la tarea de enlazar los bundles a nuestro template HTML.

Instacion:

```bash
npm i html-webpack-plugin -D
```

## Loader para CSS

MiniCssExtractPlugin
Este loader lo que nos permite es que en nuestro proyecto de desarrollo poder importar en los archivos JavaScript importar archivos CSS o de otros preprocesadores, al final webpack importara en nuestro HTML todo nuestro css.
Instalación

```bash
npm i mini-css-extract-plugin css-loader 
```