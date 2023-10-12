# Byte your Markdown
---
# Comments | Comentarios `<!--Text-->` `[Text]: #`

En realidad, Markdown no tiene una sintaxis nativa para comentarios como, por ejemplo, HTML `(<!-- comment -->)` o lenguajes de programación como Python `(# comment)` o JavaScript `(// comment)`.

Sin embargo, dado que Markdown puede ser incrustado dentro de HTML y muchos procesadores de Markdown lo interpretan y renderizan correctamente, es común ver a las personas usar la sintaxis de comentarios de HTML para agregar comentarios a sus documentos de Markdown:

<!--This is a comments-->

`<!--This is a comments-->`

[This is a comments]: #

`[This is a comments]: #`

Estos comentarios no se mostrarán en el documento renderizado, pero estarán presentes en el código fuente.

---

# Headings | Titulos `#`
En Markdown, los encabezados o "headings" se utilizan para indicar títulos y subtítulos en el documento. Markdown proporciona seis niveles de encabezados, que corresponden a los niveles de encabezados HTML `<h1>` a `<h6>`.

Para crear un encabezado en Markdown, se utiliza el carácter `#`, seguido de un espacio. El número de caracteres `#` determina el nivel del encabezado.
```md
# Titile h1
```
```html
<h1>Titile h1</h1>
```

# Titile h1

`# Titile h1`

## Titile h2

`# Titile h2`

### Titile h3

`# Titile h3`

#### Titile h4

`# Titile h4`

##### Titile h5

`# Titile h5`

###### Titile h6

`# Titile h6`

* **Semántica:** En el lenguaje de marcado HTML, los encabezados van desde `<h1>`(el más importante) hasta `<h6>` (el menos importante). Es una buena práctica usar encabezados de manera jerárquica y no saltarse niveles, ya que los encabezados también tienen importancia desde el punto de vista de la accesibilidad y la semántica del contenido.

* **Estilización:** La apariencia de los encabezados (tamaño de fuente, peso, márgenes, etc.) se determina típicamente con CSS cuando el Markdown se convierte a HTML. Sin embargo, en editores de Markdown y vistas previas, los estilos de los encabezados suelen estar predefinidos.

* **Enlace automático:** Algunos procesadores de Markdown, como los usados en GitHub, generan automáticamente enlaces anclables (o "anchor links") para cada encabezado. Esto permite a los lectores enlazar directamente a una sección específica de un documento.

* **Espacio después del #:** Es importante incluir un espacio entre el carácter # y el texto del encabezado para que se interprete correctamente como un encabezado.

---

# Text format | Formato del texto

Markdown posee su propia sintaxis para estilos como cursiva (_texto_ o *texto*), negrita (**texto**) y tachado (~~texto~~). Sin embargo, para el subrayado, se recurre al uso de HTML: <ins>texto</ins>`<ins></ins>`. Esto se debe a que Markdown no tiene una sintaxis nativa para el subrayado.


This is an _italic_ text.
```md
This is an _italic_ text.
```

This is an **strong** text.
```md
This is an **strong** text.`
```

This is an ~~strikethrough~~ text.
```md
This is an ~~strikethrough~~ text.
```

### No nativo / uso de HTML: 

This is an <ins>underlined</ins> text.
```html
This is an <ins>underlined</ins>.
```

This is an highlight <mark>highlighted</mark> text.
```html
This is an highlight <mark>highlighted</mark> text.
```

<font color="#41FAAF">This ia a text with color!</font>
```html
<font color="#41FAAF">This is a text with color!</font>
```

---

# Paragraphs | Párrafos
En Markdown, los párrafos son bloques de texto separados por una o más líneas en blanco. Es bastante sencillo y se asemeja a cómo escribimos texto en cualquier procesador de texto convencional.

I really like using Markdown.

I think I'll use it to format
all of my documents from now on.

```
I really like using Markdown.

I think I'll use it to format
all of my documents from now on.
```
---

# Line Breaks | Saltos de línea `<br>`
En Markdown, aunque la sintaxis principal para un salto de línea es añadir un "Enter", también se puede utilizar la etiqueta HTML `<br>` para lograr un resultado similar. Dado que Markdown permite la inclusión de HTML crudo, esta etiqueta se renderizará correctamente en la mayoría de los procesadores de Markdown.

I think I'll use it to format <br> all of my documents from now on.

```html
I think I'll use it to format <br> all of my documents from now on.
```

---

# Lists | Listas

## Order lists | Listas ordenadas | `1.`
Las listas ordenadas, también conocidas como listas numeradas, son una serie de elementos en un orden específico. En Markdown, las listas ordenadas se crean utilizando números seguidos de un punto y un espacio.

1. First item
2. Second item
3. Third item
   1. Indented item
   2. Indented item
4. Fourth item

`1. First item`

<br>

**Numeración automática:** En realidad, el número específico que uses para cada ítem no importa en términos de renderizado; Markdown y el HTML resultante manejarán la numeración automáticamente. Por ejemplo:
```md
1. Primer ítem
1. Segundo ítem
1. Tercer ítem
```
1. Primer ítem
1. Segundo ítem
1. Tercer ítem

<br>

**Sublistas:** Puedes anidar listas dentro de otras listas utilizando una indentación (generalmente cuatro espacios o un tabulador):
```md
1. Primer ítem
    1. Sub ítem 1
    2. Sub ítem 2
        1. Sub sub ítem 1
        1. Sub sub ítem 2
2. Segundo ítem
```
1. Primer ítem
    1. Sub ítem 1
    2. Sub ítem 2
        1. Sub sub ítem 1
        1. Sub sub ítem 2
2. Segundo ítem

<br>

**Combinar con listas no ordenadas:** Puedes combinar listas ordenadas y no ordenadas:

```md
1. Primer ítem
    - Sub ítem no ordenado
    - Otro ítem no ordenado
2. Segundo ítem
```
1. Primer ítem
    - Sub ítem no ordenado
    - Otro ítem no ordenado
2. Segundo ítem

## Unordered Lists | Listas desordenadas | `+ \ * -`
Las listas desordenadas, a menudo llamadas listas con viñetas, son una serie de elementos sin un orden numérico o secuencial específico. En Markdown, puedes crear listas desordenadas utilizando asteriscos *, signos más + o guiones -, seguidos de un espacio.

- First item
- Second item
- Third item
  - Indented item
  - Indented item
- Fourth item

`- First item`

<br>

**Sublistas:**  Al igual que con las listas ordenadas, puedes anidar listas dentro de otras listas utilizando una indentación (generalmente cuatro espacios o un tabulador)

**Combinar con listas ordenadas:** También puedes combinar listas desordenadas con listas ordenadas:

---

# Blockquote | Cita en bloque | `>`
El blockquote es una característica en Markdown que permite citar bloques de texto. Se utiliza principalmente para indicar que un fragmento de texto proviene de otra fuente o para destacar una sección particular de texto, como una cita o un comentario importante.

Sintaxis básica de Blockquote en Markdown:

Para crear un blockquote en Markdown, se precede la línea o líneas de texto con el carácter `>`:

```
> A blockquote, mark citations to other authors or documents.
>
> > Una cita en bloque, marcar citas a otros autores o documentos.
>
> 1. Ordered lists can be used
>
> - Unordered lists can be used
> - Works with various elements / Funciona con varios elementos
> - Use the character `>` to do a blockquote
```
> A blockquote, mark citations to other authors or documents.
>
> > Una cita en bloque, marcar citas a otros autores o documentos.
>
> 1. Ordered lists can be used
>
> - Unordered lists can be used
> - Works with various elements / Funciona con varios elementos
> - Use the character `>` to do a blockquote
> - Es posible anidar blockquotes utilizando múltiples caracteres >

<br>

Aunque técnicamente puedes usar blockquotes para cualquier propósito en tu documento, es recomendable usarlos para su propósito semántico: citar o destacar contenido. En la web, es común ver blockquotes estilizados de manera única, a menudo con sangrías, bordes, o fondos distintos para distinguirlos del texto principal.

---

# Code | Codigo | `` ` ` ``
En Markdown, existen diferentes maneras de representar código, ya sea código en línea o bloques de código. El código es comúnmente utilizado en documentos técnicos, tutoriales, o publicaciones relacionadas con la programación y tecnología.
## Inline Code
Para representar fragmentos cortos de código, variables, nombres de funciones, o cualquier otra entidad que quieras destacar dentro de una línea de texto, puedes utilizar acentos invertidos (backticks) ` `` `.

`print()`

Examlpe:

```md
`print()`
```

## Fenced Code Blocks | Bloques de Código

Cuando deseas representar fragmentos de código que abarcan varias líneas, usa triple acento invertido (backticks) ` ``` `:

Al encerrar tu código con tres acentos invertidos (backticks) ``` , puedes representar bloques de código que abarquen múltiples líneas.
```
    ```py
        for _ in range(5):
          print("ByteYourCode")
    ```
```

>Puedes agregar ` ```py ` ` ```html ` para indicar el lenguaje en el que estas programarlo y darle formato.

Examlpe:


Python ` ```py `

```py
for _ in range(5):
    print("ByteYourCode")
```

HTML ` ```html `

```html
<div class="row">
  <div class="youtube">
    <h1>ByteYourCode</h1>
  </div>
</div>
```

---

# Horizontal Rule | Reglas Horizontales
Las reglas horizontales en Markdown sirven como una forma visual de separar secciones de texto. Son especialmente útiles para dividir grandes bloques de texto o para indicar transiciones en el contenido.

>---

`---`

> ***

`***`

> ___

`___`

---

# Links | Enlaces `<url>` `[](url)`
Los enlaces son esenciales para conectar recursos y permitir a los lectores acceder a contenido adicional, ya sea dentro del mismo documento o en otros sitios web. En Markdown, la sintaxis para crear enlaces es sencilla y directa.

Para crear un enlace en línea, se utiliza la siguiente estructura:

My favorite chanel is [ByteYourCode by abraham_esh](https://www.youtube.com/@ByteYourCode "El mejor canal para ver tutoriales").

```md
My favorite chanel is [ByteYourCode by abraham_esh](https://www.youtube.com/@ByteYourCode "El mejor canal para ver tutoriales").
```
<br>

<https://www.youtube.com/@ByteYourCode> `<https://www.youtube.com/@ByteYourCode>`

<fake@example.com> `<fake@example.com>`

---

# Images | Imágenes `![](url)`
## Image
![This is the ByteYourCode Logo](https://yt3.googleusercontent.com/7hyuY-x_fCjYWtgITHiuoOfereaDFDM7TrLem5AXqLOqniWsVx2ZGuuXTAwGMeZ9U5Xltsp4wPw=s176-c-k-c0x00ffffff-no-rj "ByteYourCode Logo")

```md
![This is the ByteYourCode Logo](https://www.youtube.com/@ByteYourCode/img "ByteYourCode Logo")
```

## Images with link

[![This is the ByteYourCode Logo](https://yt3.googleusercontent.com/7hyuY-x_fCjYWtgITHiuoOfereaDFDM7TrLem5AXqLOqniWsVx2ZGuuXTAwGMeZ9U5Xltsp4wPw=s176-c-k-c0x00ffffff-no-rj "ByteYourCode Logo")](https://www.youtube.com/@ByteYourCode)

> Uso de imágenes locales: Además de las URLs, puedes usar rutas de archivos locales para imágenes si estás trabajando en un proyecto local o si tu archivo Markdown será visualizado en un contexto donde se pueda acceder a archivos locales.

```md
[![This is the ByteYourCode Logo](https://www.youtube.com/@ByteYourCode/img "ByteYourCode Logo")](https://www.youtube.com/@ByteYourCode)
```

## Image size

Markdown por sí mismo no tiene una sintaxis para redimensionar imágenes. Sin embargo, algunos procesadores de Markdown permiten usar HTML crudo, por lo que podrías usar etiquetas de imagen HTML para este propósito, aunque no es una solución puramente Markdown.

<img src="https://yt3.googleusercontent.com/7hyuY-x_fCjYWtgITHiuoOfereaDFDM7TrLem5AXqLOqniWsVx2ZGuuXTAwGMeZ9U5Xltsp4wPw=s176-c-k-c0x00ffffff-no-rj" width="300" height="200"> <img src="https://yt3.googleusercontent.com/7hyuY-x_fCjYWtgITHiuoOfereaDFDM7TrLem5AXqLOqniWsVx2ZGuuXTAwGMeZ9U5Xltsp4wPw=s176-c-k-c0x00ffffff-no-rj" width="200" height="300">

```html
<img src="https://theimglink.com" width="300" height="200">
```
---

# Video `<iframe>`
En Markdown puro, no hay una sintaxis específica para insertar iframe. Sin embargo, muchos procesadores de Markdown permiten incrustar HTML directamente en el contenido, lo que significa que puedes insertar un iframe usando su etiqueta HTML estándar.

<iframe width="560" height="315" src="https://www.youtube.com/embed/pBy1zgt0XPc?si=d4NdUd694V-K0EAc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

```html
<iframe width="560" height="315" src="https://www.youtube.com/embed/pBy1zgt0XPc?si=d4NdUd694V-K0EAc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
```

---

# Table | Tabla
En Markdown, las tablas permiten organizar y presentar datos de manera estructurada. La sintaxis de las tablas en Markdown es bastante directa.

| Month    | Assignee | Backup |
| -------- | -------- | ------ |
| January  | Dave     | Steve  |
| February | Gregg    | Karen  |
| March    | Diane    | Jorge  |

```
| Month    | Assignee | Backup |
| -------- | -------- | ------ |
| January  | Dave     | Steve  |
| February | Gregg    | Karen  |
| March    | Diane    | Jorge  |
```

<br>

En Markdown, las tablas permiten organizar y presentar datos de manera estructurada. La sintaxis de las tablas en Markdown es bastante directa, aunque no todos los dialectos de Markdown la soportan (sin embargo, la versión de GitHub Flavored Markdown, por ejemplo, sí lo hace).

**Ejemplo básico de una tabla en Markdown**:

```markdown
| Encabezado 1 | Encabezado 2 |
|--------------|--------------|
| fila 1, col 1 | fila 1, col 2 |
| fila 2, col 1 | fila 2, col 2 |
```

**Detalles técnicos y características**:

1. **Delimitadores**: Las columnas son separadas por el símbolo `|`.

2. **Alineación**: Puedes controlar la alineación del contenido de las columnas utilizando dos puntos `:` en la fila delimitadora. Por ejemplo:
   - `|:--------------|` alineará a la izquierda.
   - `|--------------:|` alineará a la derecha.
   - `|:-------------:|` centrará el contenido.

3. **Flexibilidad con espaciado**: El número de guiones `-` y espacios en la fila delimitadora no necesita ser exacto y no afecta la anchura final de la columna. Su propósito principal es actuar como un delimitador visual entre encabezados y contenido.

4. **Filas y columnas**: Puedes añadir tantas filas y columnas como necesites. Asegúrate de que cada fila tenga el mismo número de columnas, incluso si algunas celdas están vacías.

5. **Estilización**: La apariencia final de la tabla, como los bordes y el espaciado, dependerá del CSS aplicado en la página donde se visualice el contenido.

---

# Subscript & Superscript

En el Markdown estándar, no hay una sintaxis nativa para subíndices (subscript) o superíndices (superscript). Por eso se usa HTML.

## Subscript `<sub></sub>`

H<sub>2</sub>O

```html
H<sub>2</sub>O
```

## Superscript `<sup></sup>`

X<sup>2</sup>

```html
X<sup>2</sup>
```

---

# Heading IDs `<h3 id="id"></h3>`
Los "Heading IDs" se refieren a los identificadores únicos asociados con los encabezados en un documento HTML. Estos IDs permiten vincular directamente a una sección específica dentro de un documento, haciendo más fácil la navegación, especialmente en documentos largos.

<h3 id="custom-id">My Great Heading</h3>

```html
<h3 id="custom-id">My Great Heading</h3>
```

>El "id" en Markdown permite enlazar directamente a secciones, facilitando la navegación y compartiendo referencias precisas.
http://tudominio.com/tupagina#custom-id

---

# Indent (Tab) `&nbsp;`

&nbsp;&nbsp;&nbsp;&nbsp; This is the first sentence of my indented paragraph.

```html
&nbsp;&nbsp;&nbsp;&nbsp; This is the first sentence of my indented paragraph.
```

---

# Center `<center></center>`

<center>This text is centered.</center>


```html
<center>This text is centered.</center>
```

---

# Symbols

Copyright (©) — &copy; `&copy;`

Registered trademark (®) — &reg; `&reg;`

Trademark (™) — &trade; `&trade;`

Euro (€) — &euro; `&euro;`

Left arrow (←) — &larr; `&larr;`

Up arrow (↑) — &uarr; `&uarr;`

Right arrow (→) — &rarr; `&rarr;`

Down arrow (↓) — &darr; `&darr;`

Degree (°) — &#176; `&#176;`

Pi (π) — &#960; `&#960;`




<br> Documentación creada por @abraham_esh para ByteYourCode by abraham_esh
