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
| Todas las páginas (navbar) | Vende tu auto |---|
| Todas las páginas (navbar) | Financiamiento |---|
| Todas las páginas (navbar) | Garantia  |---|
| Todas las páginas (navbar) | Blog |---|
| Todas las páginas (navbar) | Contacto |---|
| Todas las páginas (navbar) |  |---|
|---|---|---|
|---|---|---|
|---|---|---|


## 3. Estructura semántica

## 4. Organización del CSS

```css
:root {
  /* los valores salen de DESIGN.md */

}
```

## 5. Criterios de aceptación

**Navegación**
- [ ]

**Funcionalidades**
- [ ]

**Diseño**
- [ ]

**Responsive**
- [ ]

**Accesibilidad y publicación**
- [ ]
