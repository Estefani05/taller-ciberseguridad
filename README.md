# Taller de Ciberseguridad 2025

Sitio estático en HTML que simula la página web de un evento tecnológico sobre ciberseguridad.

---

## 1) Descripción del evento
El **Taller de Ciberseguridad 2025** es un evento ficticio desarrollado como práctica académica para demostrar la correcta implementación de HTML semántico, accesibilidad y validación web.  
Incluye secciones de agenda, expositores, formulario de registro, ubicación y patrocinadores, con navegación interna y enlaces externos.

---

## 2) Estructura semántica

**Etiquetas clave y propósito:**
- `<header>` + `<nav>`: cabecera y menú de navegación interna.
- `<main>` con 5 `<section>`: Agenda, Expositores, Registro, Ubicación, Patrocinadores.
- `<article>`: ficha individual de expositor/a.
- `<figure>` + `<figcaption>`: imagen con pie descriptivo.
- `<aside>`: contenido complementario con enlace a noticia relacionada.
- `<footer>`: pie de página con derechos de autor.
- Contenido enriquecido:
  - Listas: `<ol>` y `<ul>`.
  - Cita: `<blockquote>`.
  - Tabla: `<table>` con `<thead>`, `<tbody>`, `<th>`, `<td>`.
  - Formulario: `<form>` con `<input>`, `<select>`, `<fieldset>` y `<button>`.

---

## 3) URL pública de Netlify
**URL:** https://taller-cibersegurid.netlify.app/

---

## 4) Validación W3C

**Método:** W3C Nu Validator por URL.

**Resultado:**  
La página pasó la validación sin errores.

**Captura:** `![alt text](image.png)`

---

## 5) Lighthouse

**Auditorías ejecutadas:** Accessibility y SEO sobre la URL de Netlify.

**Resultados:**
- Accessibility: **96/100**
- SEO: **91/100**

**Capturas:**
- `![alt text](image-1.png)`
- `![alt text](image-2.png)`

**Plan de mejoras:**
- Añadir `<meta name="description">` en el `<head>` para mejorar SEO.
- Revisar contraste de colores en elementos como `<blockquote>` para mantener un puntaje óptimo en accesibilidad.
- Mantener atributos `alt` descriptivos en todas las imágenes.
- Mantener etiquetas `<label>` correctamente asociadas a campos de formulario.

---

## 6) Accesibilidad aplicada

- **`tabindex`**:
  - `tabindex="0"` en imagen de Ana Pérez (enfocable por teclado).
  - `tabindex="-1"` en imagen de Carlos Gómez (excluida de la navegación por teclado, pero enfocable con JavaScript).
- **`alt`**:
  - Todas las imágenes tienen texto alternativo descriptivo.
- **`aria-*`**:
  - `aria-label="Enviar formulario de registro"` en el botón de envío.
- **Tablas**:
  - Uso de `<thead>`, `<tbody>`, `<th>` con `scope="col"`.
- **Enlaces**:
  - Texto claro y descriptivo: “Ver mapa”, “INCIBE”, evitando “haz clic aquí”.

---

### Cómo reproducir el despliegue
1. Clonar el repositorio y abrir `index.html` en un navegador.
2. Subir el proyecto a un repositorio en GitHub.
3. Conectar el repositorio a Netlify:
   - Build command: *(vacío)*  
   - Publish directory: `/`  
4. Deploy y obtener la URL pública.

---
