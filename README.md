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