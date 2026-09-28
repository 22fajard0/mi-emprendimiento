# Objetivos del usuario y funcionalidades

**Archivo:** `docs/03-funcionalidades.md` · **Fase 1** · **8 pts**

## Qué es y para qué sirve

Una **funcionalidad** es algo que el sitio debe **permitir hacer** al usuario: buscar un producto, comentar un artículo, calcular el despacho. No es una pantalla ni un botón: es la **capacidad** que ese botón o esa pantalla tienen que resolver.

Las funcionalidades conectan a tu proto-persona con el sitio:

```text
Proto-persona → Objetivo → Funcionalidad → (más adelante) Componente
Camila         → Saber si le sirve para piel sensible
               → Filtrar productos por tipo de piel
               → Filtro de categorías en la tienda
```

Si una funcionalidad no responde a ningún objetivo de tu proto-persona, probablemente no hace falta.

## Qué entregas

Una tabla con:

- Las **7 funcionalidades base** (obligatorias para todos).
- Al menos **5 funcionalidades propias** de tu emprendimiento.
- Cada una conectada a un **objetivo** de tu proto-persona y con su **prioridad**.

## Las funcionalidades base

| Parte del sitio | Funcionalidad base |
|---|---|
| **Landing** | El usuario debe poder dejar sus datos para recibir información o una oferta (**captación de leads**). Puedes reemplazarla por otra acción de conversión (cotizar, reservar, escribir por WhatsApp) si tu negocio lo justifica. |
| **Blog** | El usuario debe poder navegar los artículos por **categorías**. |
| | El usuario debe poder **comentar** un artículo. |
| | El usuario debe poder **compartir** un artículo en sus redes. |
| **E-commerce** | El usuario debe poder **buscar** productos. |
| | El usuario debe poder **filtrar** productos. |
| | El usuario debe poder **seleccionar** un producto: ver su detalle, elegir variante y agregarlo al carrito. |

Tu trabajo con estas es **adaptarlas a tu emprendimiento**: ¿filtrar por qué? ¿Qué datos pides en la captación de leads y a cambio de qué? ¿Qué variantes tiene tu producto?

## Paso a paso

### 1. Escribe los objetivos de tu proto-persona

¿Qué quiere lograr cuando entra a tu sitio? Revisa sus **necesidades y frustraciones**: casi siempre ahí están los objetivos.

### 2. Transforma cada objetivo en funcionalidad

Redáctala siempre como **"El usuario debe poder…"**. Esto te obliga a describir la capacidad y no la solución visual.

| ❌ Mal: describe una solución visual | ✅ Bien: describe una capacidad |
|---|---|
| Un botón verde grande arriba | El usuario debe poder iniciar la compra desde cualquier página |
| Un pop-up con descuento | El usuario debe poder dejar su correo a cambio de un descuento |
| Íconos de hojitas | El usuario debe poder ver los ingredientes de cada producto |

El "cómo se ve" lo decides en la Fase 2.

### 3. Adapta las 7 funcionalidades base

### 4. Agrega al menos 5 funcionalidades propias

Piensa en lo que hace distinto a tu rubro. Algunas ideas: suscribirse al newsletter, calcular el costo de despacho, guardar favoritos, ver reseñas, ver productos relacionados, consultar por WhatsApp, guía de tallas, ingredientes o información nutricional, punto de venta más cercano.

### 5. Prioriza

| Prioridad | Significa |
|---|---|
| **Imprescindible** | El sitio no cumple su objetivo sin esto |
| **Deseable** | Mejora la experiencia, pero el sitio funciona sin ella |
| **Futuro** | Buena idea, pero fuera del alcance de esta versión |

Las funcionalidades base son, en general, imprescindibles.

## Ejemplo

| Proto-persona | Objetivo | Funcionalidad | Tipo | Prioridad |
|---|---|---|---|---|
| Camila | Probar la marca sin arriesgar mucho | El usuario debe poder dejar su correo a cambio de un 10 % de descuento en su primera compra | Base (landing) | Imprescindible |
| Camila | Aprender a armar una rutina simple | El usuario debe poder navegar los artículos por categoría (rutinas, ingredientes, sustentabilidad) | Base (blog) | Imprescindible |
| Camila | Resolver dudas sobre un artículo | El usuario debe poder comentar un artículo | Base (blog) | Deseable |
| Camila | Recomendar un artículo a una amiga | El usuario debe poder compartir un artículo por WhatsApp e Instagram | Base (blog) | Deseable |
| Camila | Encontrar rápido un producto que ya conoce | El usuario debe poder buscar productos por nombre o ingrediente | Base (tienda) | Imprescindible |
| Camila | Saber si le sirve para piel sensible | El usuario debe poder filtrar productos por tipo de piel y por categoría | Base (tienda) | Imprescindible |
| Camila | Comprar el formato que necesita | El usuario debe poder ver el detalle de un producto, elegir su tamaño y agregarlo al carrito | Base (tienda) | Imprescindible |
| Camila | Saber qué se está echando en la piel | El usuario debe poder ver la lista completa de ingredientes de cada producto | Propia | Imprescindible |
| Camila | No llevarse sorpresas en el precio | El usuario debe poder calcular el costo de despacho antes de pagar | Propia | Imprescindible |
| Camila | Confiar en un producto nuevo | El usuario debe poder leer reseñas de otras clientas | Propia | Deseable |
| Camila | Comprar sin crear una cuenta | El usuario debe poder comprar como invitado | Propia | Deseable |
| Camila | Resolver una duda antes de comprar | El usuario debe poder escribir por WhatsApp desde la ficha del producto | Propia | Deseable |
| Camila | Repetir su compra habitual | El usuario debe poder suscribirse a un envío mensual | Propia | Futuro |

## Cómo usar la IA

```text
Esta es mi proto-persona: [pega tu proto-persona].
Mi sitio tiene landing, blog y tienda online de [emprendimiento].
Propón 8 funcionalidades adicionales a buscar, filtrar, seleccionar,
comentar, compartir y captar leads. Redáctalas como "El usuario debe
poder...", conéctalas con un objetivo de la proto-persona y no
describas soluciones visuales.
```

Elige las que tengan sentido para tu negocio: no tienes que usar todas.

## Errores comunes

- **Describir soluciones visuales** en vez de capacidades ("un carrusel en el inicio").
- **Funcionalidades sin objetivo**: si no sabes a qué necesidad responde, pregúntate si hace falta.
- **Copiar las base sin adaptarlas**: "el usuario debe poder filtrar" está incompleto. ¿Filtrar por qué?
- **Todo imprescindible**: si todo es prioridad, no priorizaste.

## Checklist

- [ ] Objetivos de la proto-persona
- [ ] Las 7 funcionalidades base, adaptadas a tu emprendimiento
- [ ] Mínimo 5 funcionalidades propias
- [ ] Todas redactadas como "El usuario debe poder…"
- [ ] Todas conectadas a un objetivo y con prioridad
