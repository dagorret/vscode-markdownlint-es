# Markdownlint

> Markdown/CommonMark y comprobación de estilo para Visual Studio Code
> Esta es una traducción del original: <https://github.com/DavidAnson/vscode-markdownlint/blob/main/README.md>
> La motivación de la traducción obedece a dos razones. La primera en aprender el marcado Markdown y Visual Code y la segunda proveer una traducción del documento para quien lo necesite.

## Introducción
El lenguaje de marcas [Markdown](https://es.wikipedia.org/wiki/Markdown) está diseñado para ser fácil de leer, escribir y entender. Tiene un gran éxito, y su flexibilidad es tanto un beneficio como un inconveniente. 

Muchos estilos son posibles, por lo que el formato puede ser inconsistente. Algunas construcciones no funcionan bien en todos los analizadores y deben evitarse. Por ejemplo, [aquí hay algunas construcciones de Markdown comunes y problemáticas](https://gist.github.com/DavidAnson/006a6c2a2d9d7b21b025).

[Markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint) es una extensión del código de Visual Studio que incluye una biblioteca de reglas para fomentar los estándares y la coherencia de los archivos Markdown. 

Está potenciado por [Markdownlint para Node.js](https://github.com/DavidAnson/markdownlint) que se basa en [Markdownlint para Ruby](https://github.com/mivok/markdownlint).

## Instalación

1. Abrir [Visual Studio Code](https://code.visualstudio.com/)
2. Presionar las teclas `Ctrl+P`  para cuadro de díaloho de Apertura Rápida
3. Tipear `ext install markdownlint` para buscar la extensión
4. Cliquear en el botón `Install`,  luego en el botón `Enable`

Ó

1. Escriba `Ctrl+Shift+X` para abrir las pestaña de Extensiones
2. Escriba `markdownlint` para buscar la extensión
3. Cliquear en el botón `Install`,  luego en el botón `Enable`

Ó

1. Abra una línea de comandos
2. Ejecuta `code --install-extension DavidAnson.vscode-markdownlint`
