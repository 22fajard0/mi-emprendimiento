# Arquitectura de la información — [Fajardo Motors V]

> Guía: [Arquitectura de la información](../evaluacion/guias/fase-1-requerimientos/05-arquitectura.md)

## Mapa de sitio



```text
Inicio (landing)
├── Tienda (catálogo de autos)
│   ├── Resultados con filtros (precio, marca, año, tipo, transmisión)
│   ├── Ficha del auto
│   │   ├── Galería de fotos
│   │   ├── Ficha técnica
│   │   ├── Informe de inspección Fajardo
│   │   ├── Semáforo de confianza
│   │   └── Cotizador de financiamiento
│   └── Comparador de autos
├── Vende tu auto
│   ├── Tasación en 24 h (formulario)
│   └── Consignación (cómo funciona)
├── Financiamiento
├── Garantía Fajardo
├── Blog
│   ├── Listado de artículos
│   └── Artículo
├── Quiénes somos
├── Contacto (formulario, WhatsApp, mapa y horarios)
├── Preguntas frecuentes
├── Términos y condiciones
├── Política de privacidad
└── 404 (página no encontrada)
```

## User flows

> Guía: [User flow](../evaluacion/guias/fase-1-requerimientos/06-user-flow.md)

### Flujo 1: compra

```text
`Inicio` → [Clic en "Ver autos"] → `Tienda`
→ [Aplica filtros de presupuesto, tipo y año] → `Resultados con filtros`
→ [Elige un auto] → `Ficha del auto`
→ [Revisa fotos, informe de inspección y semáforo de confianza]
→ ◇ ¿Le sirve el auto?
    ├── No → [Vuelve a la tienda o usa el comparador] → `Tienda` / `Comparador de autos`
    └── Sí → [Simula el financiamiento (opcional)] → `Cotizador de financiamiento`
        → ◇ ¿Cómo quiere avanzar?
            ├── WhatsApp → [Clic en el botón de WhatsApp] → `WhatsApp` (mensaje prellenado del auto)
            └── Visita → [Completa el formulario de visita o test drive] → `Agenda de visita`
        → `Confirmación` (contacto del equipo Fajardo Motors)
        → [Visita el local, prueba el auto y cierra la compra]

```

### Flujo 2: contenido

```text
[Busca en Google "cómo revisar un auto usado"] → `Artículo del blog`
→ [Lee el contenido: checklist, consejos y errores comunes]
→ ◇ ¿Qué hace al terminar de leer?
    ├── Quiere ver autos → [Clic en "Mira nuestros autos revisados"] → `Tienda` → continúa en Flujo 1
    ├── Quiere vender → [Clic en "Cotiza tu auto en 24 h"] → `Vende tu auto`
    ├── Quiere conversar → [Clic en "Habla con nosotros"] → `WhatsApp`
    └── Sigue leyendo → [Abre un artículo relacionado] → `Artículo del blog`

```

## Categorías

> Guía: [Categorías de productos y temas del blog](../evaluacion/guias/fase-1-requerimientos/07-categorias.md)

### Categorías de productos

| Categoría | Productos |
|---|---|
| Citycar y hatchback | Autos compactos y económicos para ciudad (ej. Chevrolet Spark, Kia Morning, Suzuki Swift) |
| Sedán | Autos familiares y de trabajo con buen maletero (ej. Hyundai Accent, Toyota Yaris, Nissan Versa) |
| SUV y crossover | Autos más altos y espaciosos para familia y ruta (ej. Hyundai Tucson, Kia Sportage, Nissan Qashqai) |
| Camionetas | Pickups para trabajo y carga (ej. Toyota Hilux, Chevrolet D-Max, Nissan NP300) |
| Furgones y comerciales | Vehículos de reparto y emprendimientos |
| Servicios | Tasación, consignación, financiamiento y garantía Fajardo |

### Categorías del blog

| Categoría | Idea de artículo | Necesidad o motivación de la proto-persona | Producto relacionado |
|---|---|---|---|
| Comprar un auto usado | Checklist para revisar un auto antes de comprar | Necesita información clara para no comprar un auto con fallas ocultas | Sedán, SUV y crossover (autos con informe de inspección) |
| Comprar un auto usado | Errores comunes al comprar un auto usado | Quiere evitar fraudes y sentir que hizo una buena compra | Semáforo de confianza e informe de inspección Fajardo |
| Papeles y trámites | Permiso de circulación y revisión técnica: cómo dejar todo al día | Quiere tener la documentación de su auto en regla desde el primer día | Autos con documentos verificadosAutos con documentos verificados |
| Financiamiento | Crédito vs. pago al contado: cuál te conviene | Quiere gastar de forma inteligente y no endeudarse de más | Financiamiento con aliados |
| Mantención y cuidado | Cada cuánto mantener tu auto y cuánto cuesta | Quiere evitar gastos altos en reparaciones y proteger a su familia | Garantía Fajardo de 3 meses |
| Mantención y cuidado | Señales de que tu auto necesita revisión urgente | Busca seguridad al manejar con su familia | Citycar, sedán y SUV (autos revisados) |
