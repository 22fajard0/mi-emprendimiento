# Spec de desarrollo — [Fajardo Motors V]

> Guía: [Spec de desarrollo](../evaluacion/guias/fase-2-specs/07-spec-de-desarrollo.md)

## Insumos y prompt para el asistente

```text
Lee DESIGN.md, docs/09-spec-diseno.md y docs/10-spec-desarrollo.md.
En la carpeta stitch/ está el código exportado de Stitch de cada pantalla.
Construye el sitio siguiendo exactamente docs/10-spec-desarrollo.md:
solo HTML y CSS, la estructura de archivos y la navegación definidas,
las variables de :root con los valores de DESIGN.md y la estructura
semántica de cada página. Usa el código de Stitch solo como referencia
visual. Al terminar, revisa cada criterio de aceptación y dime cuáles
se cumplen y cuáles no.
```

## 1. Estructura de archivos

```text
fajardo-motors/
├── index.html                  (landing)
├── tienda.html
├── ficha-producto.html
├── carrito.html                (Mi selección y visita)
├── blog.html
├── articulo.html
├── contacto.html               (incluye formulario de tasación)
├── preguntas-frecuentes.html
├── terminos.html
├── privacidad.html
├── 404.html
├── DESIGN.md
├── README.md
├── css/
│   └── styles.css
├── img/
│   ├── logo.svg
│   ├── favicon.png
│   ├── autos/                  (fotos de los autos)
│   └── blog/                   (imágenes de artículos)
├── files/
│   └── informe-inspeccion-ejemplo.pdf
├── stitch/                     (código exportado de Stitch, solo referencia)
│   ├── landing.html
│   ├── tienda.html
│   ├── ficha-producto.html
│   ├── carrito.html
│   ├── blog.html
│   └── articulo.html
└── docs/
    ├── 09-spec-diseno.md
    └── 10-spec-desarrollo.md

```

## 2. Páginas y navegación

| Desde | Elemento | Lleva a |
|---|---|---|
| Todas las páginas (navbar) | Logo “Fajardo Motors” | index.html |
| Todas las páginas (navbar) | Autos | tienda.html |
| Todas las páginas (navbar) | Vende tu auto | index.html#tasacion |
| Todas las páginas (navbar) | Financiamiento | ficha-producto.html#financiamiento |
| Todas las páginas (navbar) | Garantía | ficha-producto.html#garantia |
| Todas las páginas (navbar) | Blog | blog.html |
| Todas las páginas (navbar) | Contacto | contacto.html |
| Todas las páginas (navbar) | Botón WhatsApp | https://wa.me/<número>?text=<mensaje> (enlace externo) |
| Tienda, ficha y carrito (navbar) | Mi selección | carrito.html |
| Todas las páginas (footer) | Preguntas frecuentes | preguntas-frecuentes.html |
| Todas las páginas (footer) | Términos | terminos.html |
| Todas las páginas (footer) | Privacidad | privacidad.html |
| index.html | Botón “Ver autos” y enlace “Ver todos los autos” | tienda.html |
| index.html | Tarjeta de auto, “Ver informe” | ficha-producto.html |
| index.html | “Cotizar mi auto” | contacto.html#tasacion |
| index.html | Tarjeta de artículo, “Leer más” | articulo.html |
| tienda.html | Tarjeta de auto, “Ver informe” | ficha-producto.html |
| tienda.html | Paginación (1, 2, 3, Siguiente) | tienda.html (prototipo visual) |
| tienda.html | “Cotizar mi auto” | contacto.html#tasacion |
| ficha-producto.html | Breadcrumb “Inicio” / “Autos” | index.html / tienda.html |
| ficha-producto.html | “Agendar visita” | carrito.html |
| ficha-producto.html | “Consultar por WhatsApp” | https://wa.me/<número>?text=<auto> |
| ficha-producto.html | “Descargar informe (PDF)” | files/informe-inspeccion-ejemplo.pdf |
| ficha-producto.html | Autos similares | ficha-producto.html |
| carrito.html | “Ver informe” | ficha-producto.html |
| carrito.html | “Agendar visita” | carrito.html#confirmacion (mensaje que se muestra con :target en CSS) |
| carrito.html | “Enviar mi selección por WhatsApp” | https://wa.me/<número>?text=<selección> |
| carrito.html | “Ver autos” (estado vacío) | tienda.html |
| blog.html | Tarjeta de artículo, “Leer más” | articulo.html |
| blog.html | Chips de categoría | blog.html (prototipo visual) |
| blog.html | “Ver autos” | tienda.html |
| articulo.html | Breadcrumb “Blog” | blog.html |
| articulo.html | Índice lateral | Anclas dentro de articulo.html |
| articulo.html | “Mira nuestros autos revisados” | tienda.html |
| articulo.html | “Habla con nosotros” | https://wa.me/<número> |
| articulo.html | Artículos relacionados | articulo.html |
| 404.html | “Volver al inicio” / “Ver autos” | index.html / tienda.html |

## 3. Estructura semántica
- index.html: main con section.hero (h1), section.trust-bar, section#recien-llegados (cada auto como article.car-card), section#inspeccion (checklist y aside con el semáforo), section#tasacion y section#blog (cada tarjeta como article).
- tienda.html: main con header de sección (h1 y ordenar), aside.filters (un form con fieldset) y section.results con article.car-card. Cierra con nav aria-label="Paginación" y section#tasacion.
ficha-producto.html: nav aria-label="Breadcrumb", article con section.gallery (figure), section.summary, section#semaforo, section#informe, section#ficha-tecnica (table), section#financiamiento (form) y section#garantia. Después va aside con “Autos similares”.
carrito.html: main con section.selection (cada auto como article), aside.visit (form de agenda), section#confirmacion y un bloque de estado vacío.
- blog.html: nav aria-label="Categorías", article.featured y section.articles con article.article-card.
- articulo.html: article con header (categoría, h1, autor, fecha), figure, aside con el índice, section por cada subtítulo (h2) y section.cta. Al final, aside con relacionados.
- contacto.html: main con section#contacto (form) y section#tasacion (form de tasación).
- preguntas-frecuentes.html: main con section y preguntas en details y summary.
- terminos.html y privacidad.html: main con un article y section por apartado.
- 404.html: main con section que tiene h1, texto y botones

## 4. Organización del CSS

```css
:root {
  /* los valores salen de DESIGN.md */

  /* Colores */
  --color-primary: #1F3A5F;
  --color-secondary: #4A6FA5;
  --color-accent: #E8833A;
  --color-bg: #F7F5F0;
  --color-surface: #FFFFFF;
  --color-text: #2B2B2B;
  --color-text-muted: #6E6E6E;
  --color-success: #2E7D4F;
  --color-success-light: #3FA66B;
  --color-warning: #F2B134;
  --color-error: #B83232;

  /* Tipografía */
  --font-heading: "Poppins", sans-serif;
  --font-body: "Inter", sans-serif;
  --fs-h1: 32px;   /* desktop: 48px */
  --fs-h2: 26px;   /* desktop: 36px */
  --fs-h3: 20px;   /* desktop: 24px */
  --fs-body: 16px; /* desktop: 18px */
  --fs-button: 16px;

  /* Espaciado */
  --space-1: 4px;
  --space-2: 8px;
  --space-3: 16px;
  --space-4: 24px;
  --space-5: 40px;
  --space-6: 64px;

  /* Radios y sombras */
  --radius-sm: 8px;
  --radius-md: 16px;
  --radius-lg: 24px;
  --radius-pill: 999px;
  --shadow-card: 0 6px 16px rgba(31, 58, 95, 0.12);

  /* Layout */
  --container-max: 1200px;
  --gutter-mobile: 16px;
}

}
```

## 5. Criterios de aceptación

**Navegación**

- Las 11 páginas existen, abren sin error y usan los nombres de archivo definidos.
- La navbar y el footer tienen los mismos enlaces en todas las páginas.
- Se puede recorrer el flujo de compra: index.html → tienda.html → ficha-producto.html → carrito.html.
- Se puede recorrer el flujo de contenido: blog.html → articulo.html → tienda.html.
- Todos los enlaces internos funcionan y no hay enlaces rotos ni con # vacío, salvo los marcados como prototipo.
- Una URL inexistente muestra 404.html con enlaces para volver.
 

**Funcionalidades**

- La tienda muestra al menos 6 tarjetas de auto con foto, precio, kilometraje, transmisión y sello “Revisado”.
- Los filtros y el buscador se ven completos (prototipo visual, sin lógica).
- La ficha incluye galería, semáforo de confianza, informe de inspección, ficha técnica, cotizador y garantía.
- Los botones de WhatsApp abren wa.me con un mensaje prellenado.
- “Descargar informe (PDF)” descarga el archivo de ejemplo.
- El formulario de tasación y el de agenda de visita se ven completos (prototipo visual). “Agendar visita” muestra el mensaje de confirmación con :target.
- El semáforo comunica el estado con texto y color, no solo con color.

**Diseño**

- Todos los colores, tipografías, espaciados y radios salen de las variables de :root, sin valores sueltos en el CSS.
 Los títulos usan Poppins y los textos usan Inter.
- El botón principal usa el color de acento con texto gris carbón, nunca blanco sobre naranja.
- La tarjeta de auto se ve igual en landing, tienda y carrito (mismo componente y misma clase).
- No hay estilos inline ni CSS repetido en los HTML.

**Responsive**

- A 375 px de ancho no hay scroll horizontal en ninguna página.
- La navbar se convierte en un menú desplegable en mobile, hecho con HTML y CSS.
- Las grillas pasan de 3 o 4 columnas a 1 columna en mobile.
- Los filtros de la tienda se colapsan detrás de un botón o un details en mobile.
- El botón de WhatsApp queda flotante en mobile.
- Las imágenes se adaptan al ancho (max-width: 100%) y el HTML incluye <meta name="viewport">.

**Accesibilidad y publicación**

- Todos los HTML tienen lang="es", <title> único y meta description.
- Cada página tiene un solo <h1> y los niveles de encabezado van en orden.
- Todas las imágenes tienen alt descriptivo, y las decorativas tienen alt="".
- Todos los campos de formulario tienen label asociado.
- El contraste del texto cumple AA (mínimo 4,5:1).
- Todo se puede usar con teclado y el foco se ve claramente.
- Las rutas son relativas y el sitio funciona publicado en GitHub Pages.
- El repositorio incluye README.md con el nombre del proyecto y el enlace al sitio publicado.
