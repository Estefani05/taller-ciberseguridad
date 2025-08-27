# Taller de Ciberseguridad 2025 — Laboratorio CSS

---

## Selectores

- **Selectores de tipo**  
  Aplicados en:  
  - `header` (encabezado principal).  
  - `nav` (menú de navegación).  
  - `section` (secciones principales: agenda, expositores, registro, etc.).  
  - `img` (todas las imágenes del sitio).  
  - `p` (párrafos de contenido).  
  - `h1`, `h2`, `h3` (jerarquía de títulos).

- **Selectores de clase**  
  - `.btn` en botones de “Registrarme” y “Enviar”.  
  - `.card` en secciones de expositores.  
  - `.tag` en etiquetas de nivel o categoría.  
  - `.badge` como distintivo dentro de cada tarjeta.  
  - `.container`, `.cards-grid`, `.aside-box` para organización visual.

- **Selectores de ID**  
  - `#agenda`, `#expositores`, `#registro`, `#ubicacion`, `#patrocinadores` → secciones principales estilizadas.

- **Selectores de atributo**  
  - `a[target="_blank"]` en enlaces externos (ej. INCIBE, Ver mapa, PDF).  
  - `img[alt]` en imágenes con descripción alternativa.  
  - `input[type="email"]` en el formulario de registro.  
  - `a[href^="https://"]` en enlaces HTTPS.  
  - `a[href$=".pdf"]` en el enlace al programa del evento en PDF.

---

## Combinadores

- `nav a + a` → separa enlaces consecutivos en el menú.  
- `.card p` → estilo de párrafos dentro de tarjetas.  
- `header > nav .nav-list` → estilo directo de la lista de navegación.  
- `.tag ~ .tag` → espacio entre etiquetas consecutivas.

---

## Pseudo-clases

- **De estado**  
  - `.btn:hover` → animación al pasar el mouse.  
  - `.btn:focus-visible` → contorno accesible al navegar con teclado.  
  - `.btn:active` → efecto al hacer clic.

- **Estructurales**  
  - `.listado li:first-child` → primera entrada en negrita.  
  - `.listado li:last-child` → último elemento con opacidad reducida.  
  - `.listado li:nth-child(2n)` → elementos pares con fondo alterno.  
  - `.listado li:not(.activo)` → estilo diferente a los elementos sin clase `activo`.

---

## Otros conceptos aplicados

- **Especificidad**  
  - `!important` en `.card .badge` dentro de `overrides.css`.  
  - Estilo en línea en `<h2 class="titulo-seccion" style="margin-bottom:24px;">`.

- **Box model**  
  - Aplicado en `.card` y contenedores (`.container`, `main > section`, `.aside-box`, `.footer`) con márgenes y padding.

- **Overflow**  
  - Párrafo con clase `.overflow-demo` dentro de `.card` (control de scroll si el texto es largo).

- **Flexbox**  
  - En `header > nav .nav-list` para alinear enlaces del menú.  
  - En `.card` para apilar elementos y empujar el botón al fondo.

- **Grid**  
  - En `.cards-grid` para organizar las tarjetas de expositores en columnas.

- **Position relative/absolute**  
  - `.card { position: relative; }`  
  - `.badge { position: absolute; top: .6rem; right: .6rem; }` → destaca la etiqueta dentro de cada tarjeta.

---
