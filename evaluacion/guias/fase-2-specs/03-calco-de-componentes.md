# Calco de componentes en Whimsical

**Archivo:** `docs/07-componentes.md` + tablero en Whimsical · **Fase 2** · **4 pts**

## Qué es y para qué sirve

Un **componente** es una pieza reutilizable de una interfaz: un botón, una tarjeta de producto, un menú de navegación, un footer. Las páginas se arman combinando componentes.

**Calcar** es redibujar, en bloques simples, un componente que te gustó de otro sitio. No es copiar su diseño: es entender **cómo está construido** (qué elementos tiene, en qué orden, cómo se distribuyen) para usar esa estructura en tu propio sitio, con tu estilo.

Así cambia la pregunta: ya no es *"¿cómo hago esta página?"*, sino *"¿qué componentes necesito para construir esta página?"*.

## Qué entregas

- Un tablero en **Whimsical** con **mínimo 6 componentes** calcados, que cubran landing, blog y tienda.
- En `docs/07-componentes.md`: el link del tablero, una captura, y para cada componente: **de qué sitio lo sacaste**, **qué contiene** y **qué necesidad de tu proto-persona resuelve**.

## Paso a paso

### 1. Haz la lista de componentes que necesitas

Revisa tu mapa de sitio y tus funcionalidades. ¿Qué piezas necesita cada página? Algunos componentes típicos:

| Parte del sitio | Componentes |
|---|---|
| Todo el sitio | Navbar, footer, botón |
| Landing | Hero, sección de beneficios, formulario de captación de leads, testimonios |
| Blog | Card de artículo, filtro de categorías, bloque de compartir, comentarios |
| Tienda | Buscador, filtros, product card, ficha de producto, selector de variante, carrito |

### 2. Busca referencias

Recorre sitios de tu rubro (y de otros). Cuando un componente te llame la atención, toma una captura.

### 3. Cálcalo en Whimsical

1. Crea un tablero de **wireframes** en Whimsical (también lo usarás para el siguiente paso).
2. Pega la captura a un lado como referencia.
3. Redibuja el componente usando **rectángulos, texto y los elementos de wireframe** de Whimsical (botones, inputs, imágenes de relleno, íconos).
4. **Sin colores ni fotos**: solo estructura, en grises. El estilo lo pones después.
5. Ponle nombre a cada componente.

### 4. Documenta cada componente

Para cada uno, anota en el Markdown de dónde lo sacaste, qué contiene y qué necesidad de tu proto-persona resuelve. Esto último es lo más importante: un componente que no resuelve nada, sobra.

## Ejemplo

```markdown
# Componentes — Brote

**Tablero:** https://whimsical.com/... (link de ejemplo)

![Componentes calcados](img/componentes.png)

| Componente | Referencia | Qué contiene | Qué necesidad resuelve |
|---|---|---|---|
| Navbar | Sitio de marca de cosmética A | Logo, enlaces (Tienda, Blog, Nosotros), buscador, ícono de carrito con contador | Camila encuentra el buscador y el carrito desde cualquier página |
| Hero | Sitio de marca de café B | Título, bajada, botón principal, foto de producto | Entiende en segundos qué vende Brote y llega a la tienda |
| Formulario de leads | Sitio de marca de ropa C | Título con la oferta, campo de correo, botón, texto de privacidad | Prueba la marca con descuento sin arriesgar mucho |
| Product card | Sitio de marca de cosmética A | Imagen, nombre, etiqueta "piel sensible", precio, botón "Ver producto" | Ve precio y si le sirve sin entrar a la ficha |
| Filtros de tienda | Sitio de tienda de deportes D | Chips de categoría y lista de tipo de piel | Encuentra rápido productos para piel sensible |
| Card de artículo | Blog de revista E | Imagen, categoría, título, tiempo de lectura | Elige qué leer según su interés |
| Lista de ingredientes | Sitio de marca de cosmética F | Ícono, nombre del ingrediente, para qué sirve | Sabe exactamente qué se echa en la piel |
| Resumen del carrito | Sitio de tienda de libros G | Productos, calculadora de despacho por comuna, total, botón | No se lleva sorpresas en el precio final |
```

## Cómo usar la IA

```text
Mi sitio tiene estas páginas: [mapa de sitio] y estas funcionalidades:
[tabla]. Hazme una lista de los componentes que necesito para cada
página, qué elementos debería tener cada uno y qué tipo de sitio web
podría revisar para encontrar buenas referencias.
```

## Errores comunes

- **Pegar capturas en vez de calcar**: el ejercicio es redibujar la estructura.
- **Calcar con colores y fotos**: en esta etapa, solo estructura en grises.
- **Menos de 6 componentes**, o todos de la misma parte del sitio.
- **No explicar qué necesidad resuelve** cada uno.

## Checklist

- [ ] Mínimo 6 componentes calcados en Whimsical
- [ ] Cubren landing, blog y tienda
- [ ] Cada uno con nombre
- [ ] Link del tablero abierto y captura en `docs/img/`
- [ ] Tabla con referencia, contenido y necesidad que resuelve
