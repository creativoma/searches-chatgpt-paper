---
layout: ../../layouts/BlogPostLayout.astro
title: Truncar texto con CSS y agregar ellipsis
url: /truncar-text-mas-ellipsis
desc: Se puede truncar texto con CSS, pero no se puede agregar un ellipsis al final del texto truncado. En este post te muestro cómo hacerlo.
date: 2023-03-21
--- 

### Pregunta

Quiero truncar texto con CSS, pero no se puede agregar un ellipsis al final del texto truncado. En este post te muestro cómo hacerlo.

### Respuesta

Para truncar el texto en CSS y agregar un ellipsis al final del texto truncado, puedes utilizar la propiedad text-overflow junto con la propiedad overflow y white-space.

La propiedad text-overflow especifica cómo se muestra el contenido que se desborda fuera del área de contenido de un elemento. La propiedad overflow controla cómo se maneja el desbordamiento de contenido dentro del contenedor. La propiedad white-space controla cómo se maneja el espacio en blanco dentro del contenedor.

Para agregar un ellipsis al final del texto truncado, debes establecer text-overflow: ellipsis en el elemento, y además establecer overflow: hidden y white-space: nowrap.

Aquí te dejo un ejemplo de cómo hacerlo:

```css
.truncate {
  width: 200px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}
```

En este ejemplo, el texto se truncará si su ancho supera los 200 píxeles, y se mostrará un ellipsis al final del texto truncado.

Espero que esto te sea de ayuda. ¡Buena suerte!

### Pregunta

Ok, pero necesito que el texto se trunque en 3 líneas. ¿Cómo puedo hacerlo?

### Respuesta

Si deseas truncar el texto en 3 líneas en lugar de agregar un ellipsis, puedes usar la propiedad display junto con webkit-line-clamp y webkit-box-orient.

La propiedad display establece cómo se muestra un elemento en la página. La propiedad webkit-line-clamp establece el número máximo de líneas de texto que se mostrarán en un contenedor. La propiedad webkit-box-orient establece la dirección del eje principal de un contenedor flexible.

Aquí te dejo un ejemplo de cómo hacerlo:

```css
.truncate {
  display: -webkit-box;
  -webkit-line-clamp: 3;
  -webkit-box-orient: vertical;
  overflow: hidden;
}
```

En este ejemplo, el texto se truncará después de 3 líneas y se ocultará el exceso de contenido. Este enfoque funciona en navegadores webkit como Safari y Chrome. Si deseas que este efecto se aplique a todos los navegadores, deberás utilizar la propiedad line-clamp en lugar de webkit-line-clamp, y también agregar prefijos de proveedor para las propiedades display y box-orient.

Espero que esto te sea de ayuda. ¡Buena suerte!

### Pregunta

Gracias por la respuesta. Pero, ¿cómo puedo hacer que el texto se trunque en 3 líneas y que se muestre un ellipsis al final del texto truncado? ¿Es posible?

### Respuesta

Sí, es posible truncar el texto en 3 líneas y mostrar un ellipsis al final del texto truncado. Puedes combinar los dos enfoques que te mencioné anteriormente.

Para truncar el texto en 3 líneas y mostrar un ellipsis al final del texto truncado, puedes usar la propiedad display junto con webkit-line-clamp, webkit-box-orient, y la propiedad text-overflow.

Aquí te dejo un ejemplo de cómo hacerlo:

```css
.truncate {
  display: -webkit-box;
  -webkit-line-clamp: 3;
  -webkit-box-orient: vertical;
  overflow: hidden;
  text-overflow: ellipsis;
}
```

En este ejemplo, el texto se truncará después de 3 líneas y se mostrará un ellipsis al final del texto truncado. Este enfoque funciona en navegadores webkit como Safari y Chrome. Si deseas que este efecto se aplique a todos los navegadores, deberás utilizar la propiedad line-clamp en lugar de webkit-line-clamp, y también agregar prefijos de proveedor para las propiedades display, box-orient y text-overflow.

Espero que esto te sea de ayuda. ¡Buena suerte!