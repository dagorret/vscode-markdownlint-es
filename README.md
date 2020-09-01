# Markdownlint

> Markdown/CommonMark y comprobación de estilo para Visual Studio Code
> Esta es una traducción del original: <https://github.com/DavidAnson/vscode-markdownlint/blob/main/README.md>
>
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

## Uso

Cuando se edita un archivo de Markdown en Code con markdownlint instalado, cualquier línea que viole una de las reglas de markdownlint (ver más abajo) se activará una *Advertencia* en el editor. 

Las advertencias se indican con un subrayado verde ondulado y también pueden verse pulsando "Ctrl+Shift+M" para abrir el diálogo de errores y advertencias.

Pase el puntero del ratón por encima de una línea verde para ver la advertencia o presione "F8" y "Shift+F8" para recorrer todas las advertencias (las advertencias de markdownlint comienzan todas con "MD").

Para más información sobre una advertencia de markdownlint, coloca el cursor en una línea y haz clic en el icono de la bombilla o presiona "Ctrl+" para abrir el diálogo de acción de código. Haciendo clic en una de las advertencias del diálogo se mostrará la entrada de ayuda de esa regla en el navegador web predeterminado.

> Para un tutorial, por favor vea [Build an Amazing Markdown Editor Using Visual Studio Code and Pandoc](https://thisdavej.com/build-an-amazing-markdown-editor-using-visual-studio-code-and-pandoc/) de Dave John

## Rules

* **[MD001](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md001)** *heading-increment/header-increment* - Heading levels should only increment by one level at a time
* ~~**[MD002](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md002)** *first-heading-h1/first-header-h1* - First heading should be a top level heading~~
* **[MD003](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md003)** *heading-style/header-style* - Heading style
* **[MD004](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md004)** *ul-style* - Unordered list style
* **[MD005](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md005)** *list-indent* - Inconsistent indentation for list items at the same level
* ~~**[MD006](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md006)** *ul-start-left* - Consider starting bulleted lists at the beginning of the line~~
* **[MD007](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md007)** *ul-indent* - Unordered list indentation
* **[MD009](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md009)** *no-trailing-spaces* - Trailing spaces
* **[MD010](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md010)** *no-hard-tabs* - Hard tabs
* **[MD011](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md011)** *no-reversed-links* - Reversed link syntax
* **[MD012](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md012)** *no-multiple-blanks* - Multiple consecutive blank lines
* **[MD013](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md013)** *line-length* - Line length
* **[MD014](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md014)** *commands-show-output* - Dollar signs used before commands without showing output
* **[MD018](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md018)** *no-missing-space-atx* - No space after hash on atx style heading
* **[MD019](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md019)** *no-multiple-space-atx* - Multiple spaces after hash on atx style heading
* **[MD020](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md020)** *no-missing-space-closed-atx* - No space inside hashes on closed atx style heading
* **[MD021](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md021)** *no-multiple-space-closed-atx* - Multiple spaces inside hashes on closed atx style heading
* **[MD022](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md022)** *blanks-around-headings/blanks-around-headers* - Headings should be surrounded by blank lines
* **[MD023](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md023)** *heading-start-left/header-start-left* - Headings must start at the beginning of the line
* **[MD024](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md024)** *no-duplicate-heading/no-duplicate-header* - Multiple headings with the same content
* **[MD025](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md025)** *single-title/single-h1* - Multiple top level headings in the same document
* **[MD026](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md026)** *no-trailing-punctuation* - Trailing punctuation in heading
* **[MD027](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md027)** *no-multiple-space-blockquote* - Multiple spaces after blockquote symbol
* **[MD028](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md028)** *no-blanks-blockquote* - Blank line inside blockquote
* **[MD029](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md029)** *ol-prefix* - Ordered list item prefix
* **[MD030](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md030)** *list-marker-space* - Spaces after list markers
* **[MD031](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md031)** *blanks-around-fences* - Fenced code blocks should be surrounded by blank lines
* **[MD032](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md032)** *blanks-around-lists* - Lists should be surrounded by blank lines
* **[MD033](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md033)** *no-inline-html* - Inline HTML
* **[MD034](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md034)** *no-bare-urls* - Bare URL used
* **[MD035](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md035)** *hr-style* - Horizontal rule style
* **[MD036](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md036)** *no-emphasis-as-heading/no-emphasis-as-header* - Emphasis used instead of a heading
* **[MD037](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md037)** *no-space-in-emphasis* - Spaces inside emphasis markers
* **[MD038](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md038)** *no-space-in-code* - Spaces inside code span elements
* **[MD039](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md039)** *no-space-in-links* - Spaces inside link text
* **[MD040](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md040)** *fenced-code-language* - Fenced code blocks should have a language specified
* **[MD041](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md041)** *first-line-heading/first-line-h1* - First line in file should be a top level heading
* **[MD042](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md042)** *no-empty-links* - No empty links
* **[MD043](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md043)** *required-headings/required-headers* - Required heading structure
* **[MD044](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md044)** *proper-names* - Proper names should have the correct capitalization
* **[MD045](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md045)** *no-alt-text* - Images should have alternate text (alt text)
* **[MD046](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md046)** *code-block-style* - Code block style
* **[MD047](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md047)** *single-trailing-newline* - Files should end with a single newline character
* **[MD048](https://github.com/DavidAnson/markdownlint/blob/master/doc/Rules.md#md048)** *code-fence-style* - Code fence style

<!---
CMD-TODO: Hay que reemplzar el vínculo de abajo por uno que rediriga al respositio de Github
CMD-HECHO
-->

Vea en [la reglas de markdownlint en el archivo reglas.md](https://github.com/dagorret/vscode-markdownlint-es/blob/master/Reglas.md) para mayor detalles.

Las siguientes reglas pueden arreglarse automáticamente moviendo el cursor a una violación de la regla (texto subrayado ondulado) y tipiando "Ctrl+.` o haciendo clic en el icono de la bombilla.

* MD005 *list-indent*
* MD006 *ul-start-left*
* MD007 *ul-indent*
* MD009 *no-trailing-spaces*
* MD010 *no-hard-tabs*
* MD011 *no-reversed-links*
* MD012 *no-multiple-blanks*
* MD014 *commands-show-output*
* MD018 *no-missing-space-atx*
* MD019 *no-multiple-space-atx*
* MD020 *no-missing-space-closed-atx*
* MD021 *no-multiple-space-closed-atx*
* MD022 *blanks-around-headings*
* MD023 *heading-start-left*
* MD026 *no-trailing-punctuation*
* MD027 *no-multiple-space-blockquote*
* MD028 *no-blanks-blockquote*
* MD030 *list-marker-space*
* MD031 *blanks-around-fences*
* MD032 *blanks-around-lists*
* MD034 *no-bare-urls*
* MD037 *no-space-in-emphasis*
* MD038 *no-space-in-code*
* MD039 *no-space-in-links*
* MD044 *proper-names*
* MD047 *single-trailing-newline*.
