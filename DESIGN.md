---
version: alpha
name: "Fajardo Motors"
description: "Design system de Fajardo Motors, automotora de autos usados revisados en la región de Valparaíso: confiable, transparente y cercano."
# Guía: evaluacion/guias/fase-2-specs/06-spec-de-diseno.md
# Reemplaza TODOS los valores de ejemplo por los de tu paleta y tipografía
# (docs/08-color-tipografia.md). Los HEX van siempre entre comillas.
# Valida con: npx @google/design.md lint DESIGN.md
colors:
  primary: "#1F3A5F"
  primary-hover: "#172D4A"
  on-primary: "#FFFFFF"
  secondary: "#4A6FA5"
  on-secondary: "#FFFFFF"
  tertiary: "#E8833A"
  tertiary-hover: "#F09A57"
  on-tertiary: "#2B2B2B"
  neutral: "#F7F5F0"
  surface: "#FFFFFF"
  on-surface: "#2B2B2B"
  on-surface-variant: "#6E6E6E"
  outline: "#D9D5CB"
  disabled: "#D6D6D6"
  on-disabled: "#4A4A4A"
  success: "#2E7D4F"
  on-success: "#FFFFFF"
  success-light: "#3FA66B"
  warning: "#F2B134"
  on-warning: "#2B2B2B"
  error: "#B83232"
  on-error: "#FFFFFF"
typography:
  headline-display:
    fontFamily: "Poppins"
    fontSize: 48px
    fontWeight: 700
    lineHeight: 1.1
  headline-display-mobile:
    fontFamily: "Poppins"
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.15
  headline-lg:
    fontFamily: "Poppins"
    fontSize: 36px
    fontWeight: 600
    lineHeight: 1.2
  headline-lg-mobile:
    fontFamily: "Poppins"
    fontSize: 26px
    fontWeight: 600
    lineHeight: 1.2
  headline-md:
    fontFamily: "Poppins"
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.25
  headline-md-mobile:
    fontFamily: "Poppins"
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.25
  body-lg:
    fontFamily: "Inter"
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.6
  body-md:
    fontFamily: "Inter"
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.6
  label-md:
    fontFamily: "Poppins"
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1
rounded:
  sm: 8px
  md: 16px
  lg: 24px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  2xl: 48px
  3xl: 64px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 12px 24px
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
  button-primary-disabled:
    backgroundColor: "{colors.disabled}"
    textColor: "{colors.on-disabled}"
  button-cta:
    backgroundColor: "{colors.tertiary}"
    textColor: "{colors.on-tertiary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 12px 24px
  button-cta-hover:
    backgroundColor: "{colors.tertiary-hover}"
    textColor: "{colors.on-tertiary}"
  button-secondary:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 12px 24px
  button-whatsapp:
    backgroundColor: "{colors.success}"
    textColor: "{colors.on-success}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 12px 24px
  card-car:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
  card-article:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
  tag-verified:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.full}"
  tag-category:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.on-surface-variant}"
    rounded: "{rounded.full}"
  semaphore-ok:
    backgroundColor: "{colors.success}"
    textColor: "{colors.on-success}"
    rounded: "{rounded.sm}"
  semaphore-warning:
    backgroundColor: "{colors.warning}"
    textColor: "{colors.on-warning}"
    rounded: "{rounded.sm}"
  semaphore-error:
    backgroundColor: "{colors.error}"
    textColor: "{colors.on-error}"
    rounded: "{rounded.sm}"
  trust-bar:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
  navbar:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    padding: 16px 24px
  footer:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    padding: "{spacing.xl}"
  input-field:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 12px 14px
  message-error:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.error}"
  message-success:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.success}"
  page:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.on-surface}"
  text-secondary:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.on-surface-variant}"
---

# Fajardo Motors — Design system

## Overview

Fajardo Motors es una automotora de compra y venta de autos usados en la región de Valparaíso (Viña del Mar y Valparaíso). Su diferencial es la transparencia: cada auto se publica con informe de inspección, historial verificado y garantía de 3 meses.

La interfaz está pensada para Rodrigo Vega, de 34 años, supervisor de logística, casado y con un hijo. Busca un auto familiar confiable, investiga mucho antes de comprar, usa WhatsApp y entra sobre todo desde el celular. Su mayor miedo es que le oculten fallas.

La interfaz debe transmitir cinco sensaciones, que salen del moodboard:

- **Confiable:** una marca seria, que respalda lo que vende.
- **Transparente:** todo a la vista, sin letra chica.
- **Cercana:** trato humano, de persona a persona.
- **Segura:** protección para su familia y su inversión.
- **Porteña:** identidad local de Valparaíso y Viña del Mar.

La promesa de marca es: "Compras tranquilo: cada auto con su historial a la vista."

## Colors

- **Primary (#1F3A5F, azul profundo):** encabezados y títulos, botones principales, pie de página, sello "Revisado" y fondos de secciones destacadas. Transmite seriedad y respaldo.
- **Primary hover (#172D4A):** solo para el estado hover y foco del botón principal.
- **Secondary (#4A6FA5, azul medio):** enlaces, estados hover, íconos, etiquetas y detalles de apoyo. El texto sobre este color es blanco.
- **Tertiary (#E8833A, naranja cálido):** botones de acción (CTA) como "Ver autos", "Agendar visita" y "Cotizar mi auto", y detalles que invitan a hacer clic. El texto sobre este color es siempre gris carbón (#2B2B2B). Nunca va como color de texto.
- **Neutral (#F7F5F0, blanco cálido):** fondo general de todas las páginas.
- **Surface (#FFFFFF):** tarjetas, formularios, navbar y paneles. Se apoya sobre el fondo neutral.
- **On-surface (#2B2B2B, gris carbón):** párrafos, datos de la ficha del auto y texto sobre el acento naranja.
- **On-surface-variant (#6E6E6E):** texto secundario, como metadatos, fechas y descripciones cortas.
- **Success (#2E7D4F):** confirmaciones, botón de WhatsApp y "Todo en regla" del semáforo. Para íconos decorativos se puede usar el verde claro (#3FA66B).
- **Warning (#F2B134):** estado "Atención" del semáforo, siempre con texto gris carbón.
- **Error (#B83232):** errores de formulario y alertas del semáforo, como "Revisión técnica vencida".
- **Outline (#D9D5CB):** bordes finos y líneas divisorias.

Dónde NO se usan:
- No usar texto blanco sobre naranja (contraste 2,71:1, no cumple).
- No usar el naranja como color de texto sobre el fondo (contraste 2,49:1, no cumple).
- No usar el verde claro (#3FA66B) ni el amarillo como fondo con texto blanco.
- No comunicar un estado solo con color: el semáforo siempre lleva un texto.

## Typography

- **Títulos:** Poppins, en Bold (700) y SemiBold (600). Da firmeza y personalidad de marca.
- **Textos:** Inter, en Regular (400). Es muy legible en celular.
- **Botones:** Poppins SemiBold (600), 16 px.

| Elemento | Desktop | Mobile | Peso |
|---|---|---|---|
| h1 | 48 px | 32 px | Bold (700) |
| h2 | 36 px | 26 px | SemiBold (600) |
| h3 | 24 px | 20 px | SemiBold (600) |
| Párrafo | 18 px | 16 px | Regular (400) |
| Botón | 16 px | 16 px | SemiBold (600) |

Los tokens `headline-display`, `headline-lg`, `headline-md` y `body-lg` son los tamaños desktop. Los tokens con sufijo `-mobile` y `body-md` (16 px) son los tamaños mobile. Cada página tiene un solo h1. El texto de párrafo nunca baja de 16 px.

## Layout

- **Ancho máximo del contenido:** 1200 px, centrado.
- **Márgenes laterales:** 16 px en mobile, 24 px en tablet y 32 px en desktop.
- **Escala de espaciado:** 4, 8, 16, 24, 32, 48 y 64 px (tokens `xs` a `3xl`). Entre secciones se usan 48 o 64 px, y dentro de una tarjeta 16 px.
- **Enfoque:** mobile first.

**Breakpoints:** mobile hasta 767 px, tablet de 768 a 1023 px y desktop desde 1024 px.

| Elemento | Mobile | Tablet | Desktop |
|---|---|---|---|
| Columnas | 1 | 2 | 3 o 4 |
| Menú | Hamburguesa desplegable | Hamburguesa desplegable | Navbar horizontal con 6 enlaces y botón WhatsApp |
| Filtros de la tienda | Colapsados tras un botón "Filtros" | Colapsados tras un botón | Columna lateral fija de 250 px |
| Grilla de autos | 1 por fila (a ancho completo) | 2 por fila | 3 por fila |
| Ficha del auto | Galería arriba y datos debajo; barra inferior fija con "Consultar por WhatsApp" y "Agendar visita" | Galería y datos apilados | Galería a la izquierda y resumen a la derecha |
| Imágenes | Ancho completo, `max-width: 100%` | Ancho completo | Proporción fija 4:3 en tarjetas |
| WhatsApp | Botón flotante en la esquina inferior derecha | Botón flotante | Botón en la navbar |

## Elevation & Depth

La jerarquía se marca con capas de color y sombras suaves, sin efectos pesados:

- **Capa base:** fondo neutral (#F7F5F0).
- **Capa de tarjetas:** superficie blanca (#FFFFFF) con borde de 1 px (#D9D5CB) y sombra suave `0 6px 16px rgba(31, 58, 95, 0.12)`.
- **Elementos flotantes:** el botón de WhatsApp y la barra inferior de la ficha usan una sombra un poco más marcada, `0 8px 20px rgba(31, 58, 95, 0.20)`.
- **Hover en tarjetas:** la sombra sube un nivel y la tarjeta se desplaza 2 px hacia arriba.
- **Foco de teclado:** contorno de 3 px en azul medio (#4A6FA5) con 2 px de separación.
- **Secciones destacadas:** fondo azul profundo (#1F3A5F) con texto blanco.

## Shapes

- **Botones:** forma de píldora (`rounded.full`, 9999 px).
- **Tarjetas** (auto, artículo y barra de confianza): 16 px (`rounded.md`).
- **Inputs y filas del semáforo:** 8 px (`rounded.sm`).
- **Imágenes de tarjetas y galería:** 16 px; el bloque hero puede usar 24 px (`rounded.lg`).
- **Etiquetas y chips** ("Revisado", categorías): píldora.

## Components

### button-primary
Botón principal en azul profundo con texto blanco, para acciones de navegación importantes (por ejemplo "Descargar informe (PDF)").
- Forma de píldora, padding 12 px 24 px, Poppins SemiBold 16 px.
- **Hover:** fondo `primary-hover`. **Foco:** contorno azul medio. **Deshabilitado:** fondo gris `disabled` con texto `on-disabled`.

### button-cta
Botón de acción en naranja con texto gris carbón. Es el que más debe llamar la atención y se usa para convertir: "Ver autos", "Agendar visita", "Cotizar mi auto", "Ver informe".
- Máximo un `button-cta` por bloque visible. Nunca con texto blanco.
- **Hover:** fondo `tertiary-hover`.

### button-secondary
Botón con fondo blanco, borde azul profundo de 2 px y texto azul profundo. Para acciones alternativas ("Comparar", "Limpiar filtros", "Quitar").

### button-whatsapp
Botón verde (`success`) con texto blanco y un ícono de chat. Texto "Consultar por WhatsApp", con mensaje prellenado según la página.
- Aparece en la navbar, en la ficha, en el carrito y en el cierre de los artículos.
- En mobile existe además una versión flotante, fija en la esquina inferior derecha.

### card-car (tarjeta de auto)
Tarjeta blanca con borde y sombra suave. Se repite igual en landing, tienda, carrito y autos similares.
- **Contiene, de arriba hacia abajo:** foto, sello `tag-verified` ("Revisado") sobre la foto, marca, modelo y año (Poppins SemiBold), precio destacado (Poppins Bold, azul profundo), chips de kilometraje, transmisión y combustible, y un botón `button-cta` "Ver informe".
- El precio siempre lleva formato chileno ($7.490.000).
- **Hover:** sombra más marcada y elevación de 2 px.

### card-article (tarjeta de artículo)
Tarjeta blanca con imagen, categoría (`tag-category`), título (h3), resumen de dos líneas y enlace "Leer más" en azul medio.

### tag-verified
Sello azul profundo con texto blanco, un ícono de check y el texto "Revisado". Solo se usa en autos que ya tienen informe de inspección.

### tag-category
Chip con fondo del color neutral y texto gris secundario, para categorías del blog y características del auto (kilometraje, transmisión). Chip activo: fondo azul profundo con texto blanco.

### semaphore-ok, semaphore-warning y semaphore-error (semáforo de confianza)
Filas con un círculo de color, un título y un estado en texto.
- Verde (`success`): "Sin deudas", "Verificado". Amarillo (`warning`): "1 pendiente". Rojo (`error`): "Vencida".
- Nunca se comunica solo con color: cada fila lleva siempre el texto del estado.
- Cinco filas fijas: prendas y multas, kilometraje, mantenciones, dueños anteriores y revisión técnica.

### trust-bar (barra de confianza)
Fila de 4 ítems con ícono y texto corto: "Inspección revisada", "Historial verificado", "Garantía de 3 meses" y "Transferencia incluida". En mobile pasa a 2 columnas por 2 filas.

### navbar
Fondo blanco con borde inferior fino. Logo "Fajardo Motors" a la izquierda, seis enlaces (Autos, Vende tu auto, Financiamiento, Garantía, Blog, Contacto) y el botón `button-whatsapp` a la derecha. Enlaces en azul profundo; hover y página activa con subrayado en azul medio. En mobile se reemplaza por un menú hamburguesa.

### footer
Fondo azul profundo con texto blanco. Incluye logo, dirección (Viña del Mar), horario, WhatsApp, redes sociales y enlaces a Preguntas frecuentes, Términos y Privacidad.

### input-field
Campo con fondo blanco, borde de 1 px (#D9D5CB), radio de 8 px y texto gris carbón. Siempre con `label` visible arriba.
- **Foco:** borde y contorno azul medio. **Error:** borde rojo (#B83232) y `message-error` debajo.

### message-error y message-success
Mensajes de formulario en texto rojo o verde, siempre con un ícono y texto claro (ej. "Ingresa un teléfono válido", "¡Listo! Te confirmaremos tu visita por WhatsApp").

### page y text-secondary
`page` es el fondo general (blanco cálido) con texto gris carbón. `text-secondary` es el texto de apoyo (#6E6E6E), como fechas, metadatos y descripciones cortas.

## Do's and Don'ts

**Do**
- Usa `button-cta` (naranja con texto gris carbón) para la acción principal de cada pantalla.
- Muestra el sello "Revisado" y el semáforo en cada auto para reforzar la transparencia.
- Escribe títulos y textos reales y claros ("Compras tranquilo...", "$7.490.000").
- Mantén el mismo componente `card-car` en todas las pantallas.
- Cuida el contraste: respeta los ratios AA (mínimo 4,5:1) en todo el texto.
- Diseña primero para celular y luego amplía a tablet y desktop.
- Deja siempre visible el acceso a WhatsApp.

**Don't**
- No uses texto blanco sobre naranja ni naranja como color de texto.
- No comuniques estados solo con color; acompáñalos siempre de texto.
- No uses más de un `button-cta` por bloque visible.
- No uses sombras pesadas, degradados fuertes ni fotos con filtros extremos.
- No uses estética de "ofertón", ni autos de lujo o deportivos que contradigan la cercanía de la marca.
- No uses tamaños de texto menores a 16 px en párrafos.
- No inventes colores nuevos; si cambias uno, cámbialo primero en este archivo.
