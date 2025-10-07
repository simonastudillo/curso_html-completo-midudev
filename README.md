# Curso completo de HTML

Curso completo de HTML desde cero: SEO, semántica y más, realizado por Miguel Ángel Durán (midudev) en [YouTube](https://www.youtube.com/watch?v=3nYLTiY5skU).

## Requerimientos

- Editor de código (VSCode).
- Extensión Live Server (opcional, pero recomendable).


## HTML

- HTML es el lenguaje más importante de la web, ya que practicamente toda la web que se ve hoy en día usa HTML.
- Sus inicios se remontan a 1993 cuando Tim Berners-Lee lanzó lo que se conoce como HTML 1.0 oficialmente.
- HTML significa HyperText Markup Language (Lenguaje de Marcado de Hipertexto).
- Su función es la de estructurar el contenido de una página web, marcar el contenido (describirlo) y darle sentido.
- NO se dedica a como se ve el contenido, para eso está CSS.
- No se dedica a la lógica o comportamiento, para eso está JavaScript.


## index.html

- El archivo principal de una web es el `index.html`.
- Se llama así porque es el archivo que los servidores web buscan por defecto cuando se accede a una carpeta.
- Si no existe un `index.html`, el servidor puede mostrar un listado de archivos o un error 403 (prohibido).

## Etiquetas HTML

### Headings (h1, h2, h3, h4, h5, h6)

- Son las etiquetas de título y subtítulo.
- `h1` es el título más importante y `h6` el menos importante.
- Se recomienda usar solo un `h1` por página para el título principal.

```html
<h1>Título Principal</h1>
```
> En el ejemplo anterior `h1` es la etiqueta y `Título Principal` es el contenido, toda la linea es un elemento.

### Párrafos (p)

- Se usan para definir párrafos de texto.
- Se recomienda usar una etiqueta `p` por cada párrafo.

```html
<p>Este es un párrafo de ejemplo.</p>
```

### Strong

- Se usa para resaltar texto con importancia fuerte.
- Se recomienda usarlo para palabras clave o frases importantes.

```html
<strong>Texto importante</strong>
```

### Unordered List (ul) y List Item (li)

- `ul` se usa para listas no ordenadas (con viñetas).
- `li` se usa para cada elemento de la lista.
- Se recomienda usar listas para agrupar elementos relacionados.

```html
<ul>
  <li>Elemento 1</li>
  <li>Elemento 2</li>
  <li>Elemento 3</li>
</ul>
```

### Images (img)

- Se usa para insertar imágenes en la página.
- Es una etiqueta auto-cerrada, no tiene contenido.
- El atributo `src` define la ruta de la imagen.
- Se recomienda usar el atributo `alt` para describir la imagen, importante para SEO y accesibilidad.

```html
<img src="ruta/de/la/imagen.jpg" alt="Descripción de la imagen">
```

### Input 

- Se usa para crear campos de entrada en formularios.
- Es una etiqueta auto-cerrada.
- El atributo `type` define el tipo de campo (texto, contraseña, email, etc.).
- Se recomienda usar etiquetas `label` para describir cada campo de entrada.

```html
<label for="nombre">Nombre:</label>
<input type="text" id="nombre" placeholder="Ingrese su nombre" />
```

### Div

- Se usa para agrupar elementos y aplicar estilos o scripts.
- No tiene un significado semántico específico.

```html
<div>
   <p>Contenido dentro de un div.</p>
</div>
```

### aside

- Se usa para contenido relacionado pero no esencial, como barras laterales o anuncios.
- Tiene un significado semántico, indicando que el contenido es complementario.

```html
<aside>
   <p>Contenido adicional o relacionado.</p>
</aside>
```

### section

- Se usa para agrupar contenido relacionado en secciones temáticas.
- Tiene un significado semántico, indicando que el contenido dentro de la sección está relacionado.

```html
<section>
   <h2>Sección Título</h2>
   <p>Contenido de la sección.</p>
</section>
```

### article

- Se usa para contenido independiente y autocontenido, como artículos de blog o noticias.
- Tiene un significado semántico, indicando que el contenido puede ser distribuido o sindicado de forma independiente.

```html
<article>
   <h2>Título del Artículo</h2>
   <p>Contenido del artículo.</p>
</article>
```

### header

- Se usa para definir la cabecera de una página o sección.
- Contiene elementos como el logo, título, navegación principal, etc.
- Tiene un significado semántico, indicando que el contenido es la introducción o encabezado.

```html
<header>
   <h1>Mi Sitio Web</h1>
   <nav>
      <a href="#">Inicio</a>
      <a href="#">Sobre Nosotros</a>
      <a href="#">Contacto</a>
   </nav>
</header>
```

### footer

- Se usa para definir el pie de página de una página o sección.
- Contiene elementos como información de contacto, enlaces legales, redes sociales, etc.
- Tiene un significado semántico, indicando que el contenido es el cierre o pie de página.

```html
<footer>
   <p>&copy; 2024 Mi Sitio Web. Todos los derechos reservados.</p>
</footer>
```

### main

- Se usa para definir el contenido principal de una página.
- Solo debe haber un `main` por página.
- Tiene un significado semántico, indicando que el contenido es el foco principal de la página.

```html
<main>
   <h2>Contenido Principal</h2>
   <p>Este es el contenido más importante de la página.</p>
</main>
```

### nav

- Se usa para definir una sección de navegación.
- Contiene enlaces a otras partes del sitio o a otras páginas.
- Tiene un significado semántico, indicando que el contenido es para la navegación.

```html
<nav>
   <a href="#">Inicio</a>
   <a href="#">Servicios</a>
   <a href="#">Contacto</a>
</nav>
```

### anchor (a)

- Se usa para crear enlaces a otras páginas o secciones.
- El atributo `href` define la URL del enlace.
- Se recomienda usar texto descriptivo para el enlace.

```html
<a href="https://www.ejemplo.com">Visitar Ejemplo</a>
```

### ol

- Se usa para listas ordenadas (numeradas).
- `li` se usa para cada elemento de la lista.
- Se pueden cambiar el tipo de numeración con el atributo `type` (1, A, a, I, i).
- Se pueden numerar en orden inverso con el atributo `reversed`.
- Se puede iniciar la numeración desde un número específico con el atributo `start`.
- Se recomienda usar listas para agrupar elementos relacionados.

```html
<ol type="A" start="3" reversed>
   <li>Primer elemento</li>
   <li>Segundo elemento</li>
   <li>Tercer elemento</li>
</ol>
```

### button

- Se usa para crear botones interactivos.
- Puede contener texto o elementos HTML.
- Se recomienda usar el atributo `type` para definir el tipo de botón (button, submit, reset).

```html
<button type="button">Haz clic aquí</button>
```

### form

- Se usa para crear formularios para la entrada de datos del usuario.
- Contiene elementos como `input`, `textarea`, `select`, etc.
- Se recomienda usar el atributo `action` para definir la URL a la que se enviarán los datos del formulario.

```html
<form action="/submit" method="POST">
   <label for="email">Email:</label>
   <input type="email" id="email" name="email" required />
   <button type="submit">Enviar</button>
</form>
```

### fieldset y legend

- `fieldset` se usa para agrupar elementos relacionados dentro de un formulario.
- `legend` se usa para proporcionar un título o descripción para el grupo de elementos dentro del `fieldset`.

```html
<fieldset>
   <legend>Información Personal</legend>
   <label for="nombre">Nombre:</label>
   <input type="text" id="nombre" name="nombre" />
   <label for="edad">Edad:</label>
   <input type="number" id="edad" name="edad" />
</fieldset>
```

### label

- Se usa para definir etiquetas para elementos de formulario.
- Mejora la accesibilidad al asociar texto descriptivo con un campo de entrada.

```html
<label for="nombre">Nombre:</label>
<input type="text" id="nombre" name="nombre" />
```

### textarea

- Se usa para crear áreas de texto multilínea en formularios.
- Permite a los usuarios ingresar texto más largo que un campo de entrada estándar.

```html
<label for="mensaje">Mensaje:</label>
<textarea id="mensaje" name="mensaje" rows="4" cols="50" placeholder="Escribe tu mensaje aquí..."></textarea>
```

### select y option

- `select` se usa para crear un menú desplegable en formularios.
- `option` se usa para definir cada opción dentro del menú desplegable.

```html
<label for="pais">País:</label>
<select id="pais" name="pais">
   <option value="mx">México</option>
   <option value="es">España</option>
   <option value="ar">Argentina</option>
</select>
```

### details y summary

- `details` se usa para crear un elemento que el usuario puede expandir o contraer para ver más información.
- `summary` se usa para definir el título o encabezado del contenido que se puede expandir o contraer.

```html
<details>
   <summary>Más información</summary>
   <p>Este es el contenido adicional que se muestra al expandir.</p>
</details>
```

### video 

- Se usa para insertar contenido de video en la página web.
- Permite reproducir videos directamente en el navegador sin necesidad de plugins adicionales.

```html
<video width="320" height="240" controls>
  <source src="ruta/del/video.mp4" type="video/mp4">
  Tu navegador no soporta la etiqueta de video.
</video>
```

### audio

- Se usa para insertar contenido de audio en la página web.
- Permite reproducir archivos de audio directamente en el navegador.

```html
<audio controls>
  <source src="ruta/del/audio.mp3" type="audio/mpeg">
  Tu navegador no soporta la etiqueta de audio.
</audio>
```

### iframe

- Se usa para incrustar otro documento HTML dentro del documento actual.
- Permite mostrar contenido de otras páginas web dentro de la página actual.

```html
<iframe src="https://www.ejemplo.com" width="600" height="400"
   title="Descripción del iframe"></iframe>
```

## Atributos

- Los atributos proporcionan información adicional sobre un elemento HTML.
- Se colocan dentro de la etiqueta de apertura.
- Algunos atributos comunes son:
   - `id`: Identificador único para un elemento.
   - `name`: Nombre del elemento, útil en formularios.
   - `src`: Fuente o ruta de un recurso (como una imagen).
   - `class`: Clase o grupo al que pertenece un elemento.
   - `style`: Estilos en línea para un elemento.
   - `title`: Texto que aparece al pasar el cursor sobre el elemento.

### Atributos Globales

- Son atributos que pueden ser usados en cualquier elemento HTML.
- Algunos ejemplos son:
   - `id`
   - `class`
   - `style`
   - `title`
   - `data-*`: Atributos personalizados para almacenar datos adicionales.

### Atributos Específicos

- Son atributos que solo aplican a ciertos elementos.
- Por ejemplo:
   - `src` en la etiqueta `img`.
   - `href` en la etiqueta `a`.
   - `type` en la etiqueta `input`.
   - `alt` en la etiqueta `img`.

### Atributos Booleanos

- Son atributos que no necesitan un valor, su presencia indica que están activados.
- Algunos ejemplos son:
   - `disabled`: Deshabilita un elemento.
   - `checked`: Marca un checkbox o radio button.
   - `readonly`: Hace que un campo de entrada sea de solo lectura.
   - `required`: Indica que un campo es obligatorio en un formulario.

## Comentarios

- Se usan para agregar notas o explicaciones en el código que no se muestran en el navegador.
- Se escriben entre `<!--` y `-->`.

```html
<!-- Este es un comentario -->
<p>Este es un párrafo.</p>
<!-- Otro comentario -->
```

## Estructura

### DOCTYPE

- La declaración `<!DOCTYPE html>` se coloca al inicio del documento HTML.
- Indica al navegador que el documento está escrito en HTML5.
```html
<!DOCTYPE html>
```

### html

- La etiqueta `<html>` envuelve todo el contenido de la página.
- Se recomienda usar el atributo `lang` para especificar el idioma del contenido.

```html
<html lang="es">
```

### head

- La etiqueta `<head>` contiene metadatos y enlaces a recursos externos.
- No se muestra contenido directamente en la página.
- Se recomienda incluir:
   - `<meta charset="UTF-8">`: Define la codificación de caracteres.
   - `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: Hace que la página sea responsiva.
   - `<title>`: Define el título de la página que aparece en la pestaña del navegador.
   - Enlaces a hojas de estilo CSS y scripts JavaScript.

```html
   <link rel="stylesheet" href="styles.css">
   <script src="script.js"></script>
```

### body

- La etiqueta `<body>` contiene todo el contenido visible de la página.
- Aquí van todos los elementos como textos, imágenes, enlaces, formularios, etc.

```html
<body>
  <h1>Mi Página Web</h1>
  <p>Bienvenido a mi página web.</p>
</body>
```