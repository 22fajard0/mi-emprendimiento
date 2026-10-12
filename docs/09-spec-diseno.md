# Spec de diseño — [Fajardo Motors V]

> Guía: [Spec de diseño](../evaluacion/guias/fase-2-specs/06-spec-de-diseno.md)

La spec de diseño tiene dos partes:

1. **[`DESIGN.md`](../DESIGN.md)** (en la raíz): tu design system, en el formato que Stitch importa.
2. **Este documento:** tus pantallas, escritas como prompts listos para pegar en Stitch.

**Wireframes en Whimsical:** [https://whimsical.com/duocuc91/moodboard-fajardo-motors-v-WDmcdgHTu9Kdj187jhSME8]

> Guía de wireframes: [Wireframes](../evaluacion/guias/fase-2-specs/04-wireframes.md)

<!-- Captura de los wireframes: ![Wireframes](img/wireframes.png) -->

## Pantallas

<!-- Un prompt por pantalla. Cada uno con: pantalla y dispositivo, objetivo
de tu proto-persona, componentes de arriba hacia abajo (con los nombres de
tu DESIGN.md) y textos y datos reales. -->

### 1. Landing

```text
Pantalla: Landing de Fajardo Motors, versión desktop. Usa el design system del proyecto.
Objetivo: que Rodrigo Vega entienda en segundos que aquí compra un auto usado revisado y sin sorpresas, y avance a ver autos o a hablar por WhatsApp.
Componentes, de arriba hacia abajo:
1. Navbar: logo "Fajardo Motors", links "Autos", "Vende tu auto", "Financiamiento", "Garantía", "Blog", "Contacto" y botón "WhatsApp".
2. Hero: título "Compras tranquilo: cada auto con su historial a la vista." Subtítulo "Autos usados revisados en Viña del Mar y Valparaíso, con informe de inspección y garantía de 3 meses." Buscador rápido con selector de tipo (Citycar, Sedán, SUV, Camioneta) y presupuesto máximo, botón principal "Ver autos" y botón secundario "Habla por WhatsApp".
3. Barra de confianza: cuatro ítems con ícono: "Inspección revisada", "Historial verificado", "Garantía de 3 meses" y "Transferencia incluida".
4. Autos destacados: título "Recién llegados" y cuatro Tarjeta de auto (ej. Hyundai Accent 2019, $7.490.000, 62.000 km, Automático, sello "Revisado"), con enlace "Ver todos los autos".
5. Sección "Así revisamos cada auto": checklist del informe de inspección (Motor, Caja, Frenos, Carrocería, Documentos) junto al semáforo de confianza de ejemplo.
6. Bloque de tasación: título "Cotiza tu auto en 24 h", texto "Recibimos tu auto en parte de pago o lo vendemos por ti" y botón "Cotizar mi auto".
7. Blog: título "Consejos antes de comprar" y tres Tarjeta de artículo.
8. Footer: logo, dirección (Viña del Mar), horario, teléfono y WhatsApp, links a Preguntas frecuentes, Términos y Privacidad, y redes sociales.
Textos y datos: usa los de arriba; los datos de los autos y de contacto son de ejemplo.
```

### 2. Tienda

```text
Pantalla: Tienda de Fajardo Motors, versión desktop. Usa el design system del proyecto.
Objetivo: que Rodrigo encuentre rápido un auto familiar dentro de su presupuesto y compare opciones de un vistazo.
Componentes, de arriba hacia abajo:
1. Navbar.
2. Encabezado: título "Autos usados revisados", contador "48 autos disponibles" y selector "Ordenar por" (Menor precio, Mayor precio, Más recientes, Menor kilometraje).
3. Filtros y buscador (columna izquierda): buscador por marca o modelo, rango de precio, año, tipo de carrocería (Citycar, Sedán, SUV, Camioneta, Furgón), transmisión, combustible y botón "Limpiar filtros".
4. Grilla de Tarjeta de auto (columna derecha, 3 por fila, 9 visibles): foto, marca y modelo, año, precio, kilometraje, transmisión, sello "Revisado" y botón "Ver informe".
5. Paginación: "1 2 3 ... Siguiente".
6. Barra de confianza en versión compacta.
7. Bloque de tasación: "¿Quieres cambiar tu auto? Cotízalo en 24 h" con botón.
8. Footer.
Textos y datos: autos de ejemplo como Hyundai Accent 2019, Kia Sportage 2018 y Toyota Hilux 2017, con precios entre $5.900.000 y $16.500.000.
```

### 3. Ficha de producto

```text
Pantalla: Ficha de producto de Fajardo Motors, versión desktop. Usa el design system del proyecto.
Objetivo: dar a Rodrigo evidencia clara del estado del auto (informe, semáforo y garantía) para que decida con confianza y contacte al equipo.
Componentes, de arriba hacia abajo:
1. Navbar.
2. Breadcrumb: "Inicio > Autos > Sedán > Hyundai Accent 2019".
3. Galería de fotos (izquierda): foto principal grande y 5 miniaturas.
4. Resumen (derecha): título "Hyundai Accent 2019", precio "$7.490.000", chips "62.000 km", "Automático", "Bencina", sello "Revisado", y Botones de contacto y WhatsApp: "Consultar por WhatsApp" (mensaje prellenado del auto) y "Agendar visita".
5. Ficha con informe y semáforo: semáforo de confianza (Prendas y multas: sin deudas, Kilometraje: verificado, Mantenciones: 1 pendiente, Dueños anteriores: 3 registros, Revisión técnica: vigente) y checklist del informe de inspección (Motor, Caja de cambios, Frenos, Carrocería, Documentos) con botón "Descargar informe (PDF)".
6. Ficha técnica: tabla con año, kilometraje, motor, transmisión, combustible, color y número de dueños.
7. Cotizador de financiamiento: pie, plazo (24, 36, 48 meses) y cuota estimada, con botón "Solicitar financiamiento".
8. Garantía: "Garantía de 3 meses en motor y caja" con qué cubre.
9. Autos similares: cuatro Tarjeta de auto.
10. Footer.
Textos y datos: usa los de arriba; son datos de ejemplo.
```

### 4. Carrito

```text
Pantalla: Carrito (Mi selección y visita) de Fajardo Motors, versión desktop. Usa el design system del proyecto.
Objetivo: que Rodrigo revise los autos que guardó y dé el siguiente paso: agendar una visita o conversar por WhatsApp.
Componentes, de arriba hacia abajo:
1. Navbar con contador de autos guardados.
2. Título "Mi selección (2 autos)".
3. Lista de autos guardados (columna izquierda): versión compacta de la Tarjeta de auto con foto, nombre, precio, kilometraje, sello "Revisado", botón "Ver informe" y enlace "Quitar".
4. Resumen y agenda (columna derecha): título "Agenda tu visita", selector de fecha y hora, nombre, teléfono, comentario opcional, botón principal "Agendar visita" y botón secundario "Enviar mi selección por WhatsApp".
5. Barra de confianza con "Garantía de 3 meses" y "Transferencia incluida".
6. Estado vacío: mensaje "Aún no guardas autos" con botón "Ver autos".
7. Footer.
Textos y datos: dos autos de ejemplo (Hyundai Accent 2019 por $7.490.000 y Kia Sportage 2018 por $12.900.000).
```

### 5. Blog

```text
Pantalla: Blog de Fajardo Motors, versión desktop. Usa el design system del proyecto.
Objetivo: que quien busca consejos antes de comprar un auto usado encuentre el artículo que necesita y luego pase a la tienda.
Componentes, de arriba hacia abajo:
1. Navbar.
2. Encabezado: título "Blog Fajardo Motors" y subtítulo "Consejos para comprar, vender y cuidar tu auto".
3. Filtros por categoría: "Todos", "Comprar un auto usado", "Papeles y trámites", "Financiamiento", "Mantención y cuidado", "Vender tu auto" y "Novedades".
4. Artículo destacado: Tarjeta de artículo grande con imagen, categoría, título "Checklist para revisar un auto antes de comprar", resumen y botón "Leer más".
5. Grilla de seis Tarjeta de artículo (3 por fila): imagen, categoría, título, resumen de dos líneas y "Leer más".
6. Llamado a la acción: "¿Listo para ver autos revisados?" con botón "Ver autos" y botón de WhatsApp.
7. Footer.
Textos y datos: títulos de ejemplo como "Errores comunes al comprar un auto usado", "Cómo calcular el pie y la cuota de tu auto" y "Consignación vs. venta directa".
```

### 6. Artículo

```text
Pantalla: Artículo del blog de Fajardo Motors, versión desktop. Usa el design system del proyecto.
Objetivo: que Rodrigo lea un consejo útil sobre cómo revisar un auto usado y, al terminar, pase a ver autos o escriba por WhatsApp.
Componentes, de arriba hacia abajo:
1. Navbar.
2. Breadcrumb: "Inicio > Blog > Comprar un auto usado".
3. Encabezado del artículo: etiqueta de categoría, título "Checklist para revisar un auto antes de comprar", autor "Equipo Fajardo Motors", fecha "12 de octubre de 2026" y tiempo de lectura "5 min".
4. Imagen principal del artículo.
5. Índice lateral con los apartados del artículo.
6. Contenido: introducción, subtítulos (h2) y checklist de 8 puntos (documentos, kilometraje, carrocería, motor, frenos, neumáticos, luces, prueba de manejo), con un recuadro destacado "Consejo: pide siempre el informe de inspección".
7. Llamado a la acción en artículo: título "Compra con la tranquilidad de un auto revisado", botón "Mira nuestros autos revisados" y botón "Habla con nosotros" (WhatsApp).
8. Artículos relacionados: tres Tarjeta de artículo.
9. Footer.
Textos y datos: usa los de arriba; el contenido del artículo puede ser texto de ejemplo.Pantalla: Artículo del blog de Fajardo Motors, versión desktop. Usa el design system del proyecto.
Objetivo: que Rodrigo lea un consejo útil sobre cómo revisar un auto usado y, al terminar, pase a ver autos o escriba por WhatsApp.
Componentes, de arriba hacia abajo:
1. Navbar.
2. Breadcrumb: "Inicio > Blog > Comprar un auto usado".
3. Encabezado del artículo: etiqueta de categoría, título "Checklist para revisar un auto antes de comprar", autor "Equipo Fajardo Motors", fecha "12 de octubre de 2026" y tiempo de lectura "5 min".
4. Imagen principal del artículo.
5. Índice lateral con los apartados del artículo.
6. Contenido: introducción, subtítulos (h2) y checklist de 8 puntos (documentos, kilometraje, carrocería, motor, frenos, neumáticos, luces, prueba de manejo), con un recuadro destacado "Consejo: pide siempre el informe de inspección".
7. Llamado a la acción en artículo: título "Compra con la tranquilidad de un auto revisado", botón "Mira nuestros autos revisados" y botón "Habla con nosotros" (WhatsApp).
8. Artículos relacionados: tres Tarjeta de artículo.
9. Footer.
Textos y datos: usa los de arriba; el contenido del artículo puede ser texto de ejemplo.
```

### Versión mobile (para cada pantalla)

```text
Genera la versión mobile (375px de ancho) de esta pantalla siguiendo la
sección Layout del design system: 
```
