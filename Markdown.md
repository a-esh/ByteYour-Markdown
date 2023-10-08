# Markdown

# Comments | Comentarios `<!---->` `[]: #`

<!--This is a comments-->

`<!--This is a comments-->`

[This is a comments]: #

`[This is a comments]: #`

---

# Headings | Titulos `#`

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

## Fenced Code Blocks

Enter your code between ` ``` ` for multi-line codes | Introduzca su código entre ` ``` ` para códigos multilínea

You can add ` ```py ` ` ```html ` to indicate the language in which you are programming and formatting it.

Puedes agregar ` ```py ` ` ```html ` para indicar el lenguaje en el que estas programarlo y darle formato

Examlpe:

Python ` ```py `

```py
for _ in range(5):
    print("DeepDev")
```

HTML ` ```html `

```html
<div class="row">
  <div class="youtube">
    <h1>DeepDev</h1>
  </div>
</div>
```

---

# Horizontal Rule

>---

`---`

> ***

`***`

> ___

`___`

---

# Links | Enlaces `<url>` `[](url)`

My favorite chanel is [DeepDev by A-esh](https://www.youtube.com/@DeepDevbyA-esh "El mejor canal para ver tutoriales").

```md
My favorite chanel is [DeepDev by A-esh](https://www.youtube.com/@DeepDevbyA-esh "El mejor canal para ver tutoriales").
```

<https://www.youtube.com/@DeepDevbyA-esh> `<https://www.youtube.com/@DeepDevbyA-esh>`

<fake@example.com> `<fake@example.com>`

# Images `![](url)`

![This is the DeepDev Logo](https://yt3.googleusercontent.com/aT4oqhktsxW97jFugSDBjOMsflNTo53wU6-NxYZo_5EJVs9Eh83LMWactzrrVg8zD7Mx3ZxLiQ=s176-c-k-c0x00ffffff-no-rj "DeepDev Logo")

```md
![This is the DeepDev Logo](https://yt3.googleusercontent.com/aT4oqhktsxW97jFugSDBjOMsflNTo53wU6-NxYZo_5EJVs9Eh83LMWactzrrVg8zD7Mx3ZxLiQ=s176-c-k-c0x00ffffff-no-rj "DeepDev Logo")
```

Images with link

[![This is the DeepDev Logo](https://yt3.googleusercontent.com/aT4oqhktsxW97jFugSDBjOMsflNTo53wU6-NxYZo_5EJVs9Eh83LMWactzrrVg8zD7Mx3ZxLiQ=s176-c-k-c0x00ffffff-no-rj "DeepDev Logo")](https://www.youtube.com/@DeepDevbyA-esh)

```md
[![This is the DeepDev Logo](https://yt3.googleusercontent.com/aT4oqhktsxW97jFugSDBjOMsflNTo53wU6-NxYZo_5EJVs9Eh83LMWactzrrVg8zD7Mx3ZxLiQ=s176-c-k-c0x00ffffff-no-rj "DeepDev Logo")](https://www.youtube.com/@DeepDevbyA-esh)
```

Image size

<img src="https://yt3.googleusercontent.com/aT4oqhktsxW97jFugSDBjOMsflNTo53wU6-NxYZo_5EJVs9Eh83LMWactzrrVg8zD7Mx3ZxLiQ=s176-c-k-c0x00ffffff-no-rj" width="200" height="200">

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

# Subscript `<sub></sub>`

H<sub>2</sub>O
H~2~O

# Superscript `<sup></sup>`

X<sup>2</sup>

some Markdown processors allow
X^2^

# Highlight `<mark></mark>`

I need to highlight these ==very important words==.

I need to highlight these <mark>very important words</mark>.

# Heading IDs `<h3 id="id"></h3>`

<h3 id="custom-id">My Great Heading</h3>

### My Great Heading {#custom-id}

# Indent (Tab) `&nbsp;`

&nbsp;&nbsp;&nbsp;&nbsp; This is the first sentence of my indented paragraph.

`&nbsp;&nbsp;&nbsp;&nbsp; This is the first sentence of my indented paragraph.`

# Center `<center></center>`

<center>This text is centered.</center>

<center>

```md
<center>This text is centered.</center>
```

</center>

# Color `<font></font>`

<font color="#41FAAF">This ia a text with color!</font>

```md
<font color="#41FAAF">This is a text with color!</font>
```

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

Documentación creada por A-esh para DeepDev by A-esh
