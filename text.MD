
---

## 📘 Fundamentos de HTML

---

### 📌 ¿Qué es HTML?

HTML significa **HyperText Markup Language** o “Lenguaje de Marcado de Hipertexto”. Es el lenguaje principal para **estructurar y organizar el contenido de las páginas web**. No es un lenguaje de programación porque no contiene lógica ni algoritmos, sino que funciona como un conjunto de **etiquetas** que describen los elementos de un sitio web: textos, imágenes, formularios, videos, enlaces, etc.

HTML utiliza un sistema de etiquetas encerradas entre corchetes angulares (`< >`). Estas etiquetas suelen venir en pares: una etiqueta de apertura `<etiqueta>` y una de cierre `</etiqueta>`. El contenido va en medio.

Ejemplo:

```html
<p>Este es un párrafo en HTML.</p>
```

---

### 🔹 ¿Qué es el DOCTYPE y la estructura básica?

Antes de escribir cualquier contenido, es necesario indicar al navegador que el documento es HTML5 (la versión actual más común) usando la declaración `<!DOCTYPE html>`. Después, se coloca la etiqueta raíz `<html>`, y dentro de ella dos secciones principales: `<head>` y `<body>`.

**Estructura mínima de una página HTML:**

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
    <title>Mi primera página HTML</title>
  </head>
  <body>
    <h1>¡Bienvenido a HTML!</h1>
    <p>Este es un párrafo inicial.</p>
  </body>
</html>
```

🔎 **Desglose de la estructura:**

* **<!DOCTYPE html>**: Indica que se trata de un documento HTML5.
* **<html>**: La raíz de toda la página web.
* **<head>**: Contiene información **meta** (que no se ve en la página), como el título de la pestaña, codificación de caracteres, enlaces a CSS, scripts, etc.
* **<meta charset="UTF-8">**: Define la codificación de caracteres. Es importante para que se muestren correctamente caracteres especiales como tildes y eñes.
* **<title>**: Título que aparece en la pestaña del navegador.
* **<body>**: Contiene todo el contenido visible de la página.

---

### 🏗️ Etiquetas esenciales de HTML

Estas son las **etiquetas básicas** que permiten crear casi cualquier estructura inicial para un sitio web:

---

#### 🔖 Encabezados: `<h1>` a `<h6>`

Se usan para definir títulos y jerarquías de contenido.

* `<h1>` es el título principal y el más importante (solo uno por página recomendado).
* `<h2>` a `<h6>` son subtítulos de menor importancia.

```html
<h1>Título principal</h1>
<h2>Subtítulo</h2>
<h3>Sección</h3>
```

**Tip SEO:** Los buscadores como Google usan los encabezados para entender la estructura de tu contenido.

---

#### 📄 Párrafos: `<p>`

Representan bloques de texto corrido.

```html
<p>Este es un párrafo que describe información importante.</p>
```

---

#### 🔗 Enlaces: `<a>`

Sirven para crear hipervínculos a otras páginas o sitios web. El atributo `href` indica la dirección de destino.

```html
<a href="https://www.google.com">Visita Google</a>
```

Puedes enlazar a:

* URLs externas (`https://...`)
* Archivos internos (ej. `pagina2.html`).
* Secciones de la misma página (anclas: `href="#seccion"`).

---

#### 🖼️ Imágenes: `<img>`

Se usan para mostrar imágenes.

* Atributo `src`: ruta de la imagen.
* Atributo `alt`: texto alternativo (importante para accesibilidad y SEO).

```html
<img src="foto.jpg" alt="Descripción de la imagen">
```

---

#### 📋 Listas: `<ul>`, `<ol>`, `<li>`

* `<ul>`: Lista desordenada (viñetas).
* `<ol>`: Lista ordenada (numerada).
* `<li>`: Elemento de lista.

```html
<ul>
  <li>Elemento 1</li>
  <li>Elemento 2</li>
</ul>

<ol>
  <li>Paso 1</li>
  <li>Paso 2</li>
</ol>
```

---

#### 📦 Contenedores: `<div>` y `<span>`

Se usan para agrupar y organizar elementos:

* `<div>`: contenedor en bloque (ocupa todo el ancho disponible).
* `<span>`: contenedor en línea (dentro de párrafos u otros textos).

```html
<div>
  <h2>Sección de contenido</h2>
  <p>Texto dentro de un div.</p>
</div>

<p>Este es un texto con <span style="color: red;">palabra destacada</span>.</p>
```

---

#### 📝 Formularios básicos: `<form>`, `<input>`, `<button>`

Los formularios permiten a los usuarios enviar información al sitio web.

```html
<form>
  <label for="nombre">Nombre:</label>
  <input type="text" id="nombre" placeholder="Escribe tu nombre">
  <button type="submit">Enviar</button>
</form>
```

Atributos comunes en `<input>`:

* `type`: especifica el tipo de entrada (texto, email, password, checkbox, etc.).
* `placeholder`: texto guía dentro del campo.
* `id`: identificador único para asociar etiquetas `<label>`.

---

### ✅ Buenas prácticas iniciales

🔹 Siempre usa etiquetas semánticas y jerarquía de encabezados adecuada (un solo `<h1>`, y de ahí descendente).

🔹 Usa el atributo `alt` en imágenes para mejorar accesibilidad y SEO.

🔹 Valida tu HTML con [W3C Validator](https://validator.w3.org/) para aprender de tus errores.

🔹 Organiza tu código con sangrías para mayor claridad y mantenimiento.

---

### 🎨 Ejercicio práctico

1️⃣ Crea un archivo llamado `index.html`.
2️⃣ Escribe el siguiente contenido:

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
    <title>Mi primera página</title>
  </head>
  <body>
    <h1>¡Hola mundo!</h1>
    <p>Este es mi primer sitio web hecho con HTML.</p>

    <h2>Mis hobbies</h2>
    <ul>
      <li>Leer</li>
      <li>Programar</li>
      <li>Jugar fútbol</li>
    </ul>

    <h2>Contacto</h2>
    <form>
      <label for="email">Tu correo:</label>
      <input type="email" id="email" placeholder="ejemplo@correo.com">
      <button type="submit">Enviar</button>
    </form>
  </body>
</html>
```

3️⃣ Abre el archivo con tu navegador y observa cómo aparece.

---

### 📚 Recursos recomendados

* [MDN HTML Reference](https://developer.mozilla.org/es/docs/Web/HTML) – Guía oficial con ejemplos.
* [W3Schools HTML Tutorial](https://www.w3schools.com/html/) – Tutorial interactivo paso a paso.
* [FreeCodeCamp Curso HTML en Español](https://www.youtube.com/watch?v=ELSm-G201Ls) – Curso en video.

