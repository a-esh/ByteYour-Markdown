# Byte your Markdown
---
# Comments | Comentarios `<!--Text-->` `[Text]: #`

<!--This is a comments-->

`<!--This is a comments-->`

[This is a comments]: #

`[This is a comments]: #`

> Comments are hidden in the view | Los comentarios se ocultan en la vista

---

# Headings | Titulos `#`

# Title h1

`# Title h1`

## Title h2

`# Title h2`

### Title h3

`# Title h3`

#### Title h4

`# Title h4`

##### Title h5

`# Title h5`

###### Title h6

`# Title h6`

---

# Text format | Formato del texto

This is an _italic_ text.

`This is an _italic_ text.`

This is an **strong** text.

`This is an **strong** text.`

This is an ~~strikethrough~~ text.

`This is an ~~strikethrough~~ text.`

This is an <ins>underlined</ins> text.

`This is an <ins>underlined</ins>.`

---

# Paragraphs | Párrafos

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

I think I'll use it to format <br> all of my documents from now on.

```html
I think I'll use it to format <br> all of my documents from now on.
```

---

# Lists | Listas

## Order lists | Listas ordenadas | `1.`

1. First item
2. Second item
3. Third item
   1. Indented item
   2. Indented item
4. Fourth item

`1. First item`

## Unordered Lists | Listas desordenadas | `+ \ * -`

- First item
- Second item
- Third item
  - Indented item
  - Indented item
- Fourth item

`- First item`

---

# Blockquote | Cita en bloque | `>`

> A blockquote, mark citations to other authors or documents.
>
> > Una cita en bloque, marcar citas a otros autores o documentos.
>
> 1. Ordered lists can be used
>
> - Unordered lists can be used
> - Works with various elements / Funciona con varios elementos
> - Use the character `>` to do a blockquote

---

# Code | Codigo | `` ` ` ``
## Inline Code
`` Use `code` in your Markdown file. ``
`` Usa `code` en tu archivo Markdown. ``

Examlpe:

```
`` Use `code` in your Markdown file. ``
```

## Fenced Code Blocks | Bloques de Código

Enter your code between ` ``` ` for multi-line codes | Introduzca su código entre ` ``` ` para códigos multilínea

>You can add ` ```py ` ` ```html ` to indicate the language in which you are programming and formatting it.

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

>---

`---`

> ***

`***`

> ___

`___`

---

# Links | Enlaces `<url>` `[](url)`

My favorite chanel is [ByteYourCode by abraham_esh](https://www.youtube.com/@ByteYourCode "El mejor canal para ver tutoriales").

```md
My favorite chanel is [ByteYourCode by abraham_esh](https://www.youtube.com/@ByteYourCode "El mejor canal para ver tutoriales").
```

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

```md
[![This is the ByteYourCode Logo](https://www.youtube.com/@ByteYourCode/img "ByteYourCode Logo")](https://www.youtube.com/@ByteYourCode)
```

## Image size

<img src="https://yt3.googleusercontent.com/7hyuY-x_fCjYWtgITHiuoOfereaDFDM7TrLem5AXqLOqniWsVx2ZGuuXTAwGMeZ9U5Xltsp4wPw=s176-c-k-c0x00ffffff-no-rj" width="300" height="200"> <img src="https://yt3.googleusercontent.com/7hyuY-x_fCjYWtgITHiuoOfereaDFDM7TrLem5AXqLOqniWsVx2ZGuuXTAwGMeZ9U5Xltsp4wPw=s176-c-k-c0x00ffffff-no-rj" width="200" height="300">

```html
<img src="https://theimglink.com" width="300" height="200">
```
---

# Video 

<iframe width="560" height="315" src="https://www.youtube.com/embed/pBy1zgt0XPc?si=d4NdUd694V-K0EAc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

```html
<iframe width="560" height="315" src="https://www.youtube.com/embed/pBy1zgt0XPc?si=d4NdUd694V-K0EAc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
```

---

# Table | Tabla

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

---

# Script

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

# Highlight `<mark></mark>`

I need to highlight these <mark>very important words</mark>.
```html
I need to highlight these <mark>very important words</mark>.
```

---

# Heading IDs `<h3 id="id"></h3>`

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

# Color `<font></font>`

<font color="#41FAAF">This isa text with color!</font>

```html
<font color="#41FAAF">This is a text with color!</font>
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
