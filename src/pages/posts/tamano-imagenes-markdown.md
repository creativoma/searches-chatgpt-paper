---
layout: ../../layouts/BlogPostLayout.astro
title: Tamaño de imagenes en markdown
url: /tamano-imagenes-markdown
desc: ¿Se puede cambiar el tamaño de las imágenes que agregamos en Markdown?
date: 2023-04-05
--- 

### Pregunta

¿Se puede cambiar el tamaño de las imágenes que agregamos en Markdown?

### Respuesta

Sí, se puede cambiar el tamaño de las imágenes que agregamos en Markdown utilizando la sintaxis HTML. En Markdown, puedes agregar una imagen usando el siguiente formato:

```markdown
![Texto alternativo de la imagen](ruta/a/la/imagen.jpg)
```

Para cambiar el tamaño de la imagen, se puede utilizar el atributo width en la etiqueta <img> de HTML. Para hacer esto, debes escribir el siguiente código:

```html
<img src="ruta/a/la/imagen.jpg" alt="Texto alternativo de la imagen" width="400"/>
```

En el ejemplo anterior, se ha especificado que la imagen debe tener un ancho de 400 píxeles. Puedes cambiar el número para ajustar el tamaño de la imagen según tus necesidades.

### Pregunta

Entiendo, pero quiero hacerlo en un archivo Markdown. ¿Cómo puedo hacerlo?

### Respuesta

Lamentablemente, no es posible cambiar el tamaño de una imagen directamente en un archivo Markdown sin recurrir a HTML. La sintaxis de Markdown no ofrece una forma nativa de establecer el tamaño de una imagen.

Sin embargo, si estás utilizando un procesador de texto como Microsoft Word o Google Docs para escribir el archivo Markdown, puedes ajustar el tamaño de la imagen antes de copiarla y pegarla en el archivo. También puedes utilizar un editor de imágenes para cambiar el tamaño de la imagen antes de incluirla en tu archivo Markdown.

En resumen, si deseas cambiar el tamaño de una imagen directamente en un archivo Markdown, tendrás que utilizar HTML o cambiar el tamaño de la imagen antes de incluirla en tu archivo.