# QA y coherencia

**Archivo:** `docs/11-qa.md` · **Fase 3** · **5 pts QA + 4 pts coherencia**

## Qué es y para qué sirve

**QA** (quality assurance, aseguramiento de calidad) es revisar si lo que construiste **cumple lo que dijiste que ibas a construir**. Generar el sitio no significa que esté terminado.

```text
SPEC        Lo que debería ocurrir
  ↓
RESULTADO   Lo que realmente ocurrió
  ↓
GAP         La diferencia entre ambos
```

La **coherencia** es la pregunta más importante de toda la evaluación: ya no es *"¿quedó bonito?"*, sino **"¿cumple lo que debía resolver?"**.

## Qué entregas

En `docs/11-qa.md`:

1. El **link de Stitch** y las **capturas** del prototipo (de la guía anterior).
2. La **tabla de QA**: cada criterio de aceptación de tu spec de desarrollo, si se cumplió y qué corregiste.
3. La **reflexión de coherencia**: el recorrido de tus user flows en el sitio y cómo el resultado responde al brief y a tu proto-persona.

## Paso a paso

### 1. Copia tus criterios de aceptación

Toma la lista de criterios de tu spec de desarrollo y pásala a una tabla.

### 2. Revisa uno por uno

Abre tu sitio y verifica cada criterio. Sé honesta u honesto: un ❌ que corregiste vale más que un ✅ que no revisaste.

### 3. Corrige y documenta

Para cada ❌, corrige el sitio y anota qué hiciste. Si decidiste **no** corregirlo, o cambiar la spec, explica por qué.

| Resultado | Significa |
|---|---|
| ✅ | Se cumplió a la primera |
| ❌ → ✅ | No se cumplía y lo corregiste |
| ❌ | No se cumple; explica por qué |

### 4. Recorre tus user flows

Haz cada flujo en el sitio publicado, paso a paso, como si fueras tu proto-persona. Anota si se pudo completar.

### 5. Escribe la reflexión de coherencia

En 5 a 10 líneas, responde:

- ¿Cómo responde el sitio al **objetivo** que definiste en el brief?
- ¿Qué **necesidades y frustraciones** de tu proto-persona resuelve, y con qué?
- ¿Qué **cambió** entre la Fase 1 y el sitio final, y por qué?

## Ejemplo

```markdown
# QA — Brote

## Prototipo en Stitch

**Proyecto:** https://stitch.withgoogle.com/... (link de ejemplo)

![Landing](img/stitch-landing.png)
![Tienda](img/stitch-tienda.png)

## Revisión de criterios de aceptación

| Criterio | Resultado | Corrección |
|---|---|---|
| La navbar y el footer son iguales en todas las páginas | ❌ → ✅ | En blog.html faltaba el enlace al carrito; copié la navbar de index.html |
| El precio es visible en todas las product cards | ✅ | — |
| En mobile la tienda muestra 1 producto por fila | ❌ → ✅ | Agregué una media query en styles.css |
| No hay scroll horizontal en 375 px | ❌ → ✅ | La imagen del hero tenía ancho fijo; la cambié a max-width: 100% |
| Todas las imágenes tienen alt | ❌ → ✅ | Faltaba en 4 imágenes del blog |
| Todos los colores salen de las variables | ❌ → ✅ | Stitch traía colores escritos a mano; los reemplacé por variables |
| El filtro por tipo de planta funciona | ❌ | Es un prototipo visual, como se declaró en 04-tecnologias.md |

## User flows

| Flujo | ¿Se completa? | Observación |
|---|---|---|
| Compra: Instagram → landing → tienda → producto → carrito | ✅ | — |
| Contenido: artículo → producto → carrito | ❌ → ✅ | El producto recomendado del artículo no tenía enlace; lo agregué |

## Coherencia

El objetivo del brief era vender online a clientes de todo Chile, y el sitio
permite llegar al carrito en 4 clics desde Instagram. La frustración principal
de Camila era que se le mueren las plantas sin saber por qué: el blog tiene
guías de cuidado, cada ficha explica para qué plantas sirve el producto y cómo
usarlo, y el diagnóstico por síntoma la lleva de "hojas amarillas" a la
solución. Para su miedo a un despacho caro, el carrito tiene calculadora por comuna.

Lo que cambió: en la Fase 1 pensamos en una sección de testimonios en la
landing, pero en los wireframes vimos que alargaba mucho la página en el
celular; la reemplazamos por una sección "Plantas fáciles para empezar", que
responde mejor a su motivación de tener una casa bonita con plantas.
```

## Errores comunes

- **Todo ✅ sin haber revisado**: un QA sin correcciones es sospechoso.
- **Revisar solo el diseño** y no los flujos, el responsive o la accesibilidad.
- **Una reflexión genérica** ("el sitio cumple con todo lo solicitado") sin mencionar a la proto-persona ni el brief.
- **No explicar los cambios** entre lo planificado y lo construido.

## Checklist

- [ ] Link de Stitch y capturas
- [ ] Tabla con todos los criterios de aceptación y su resultado
- [ ] Correcciones documentadas
- [ ] Los dos user flows recorridos en el sitio
- [ ] Reflexión de coherencia con el brief y la proto-persona
- [ ] Cambios respecto a la Fase 1 explicados
