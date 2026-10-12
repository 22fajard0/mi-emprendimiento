# Tecnologías del proyecto — [Fajardo Motors V]

> Guía: [Tecnologías del proyecto](../evaluacion/guias/fase-1-requerimientos/04-tecnologias.md)

## Stack

| Área | Herramienta | Para qué la uso |
|---|---|---|
| Construcción | HTML + CSS | Estructurar y dar estilo a las páginas del sitio (inicio, catálogo, ficha del auto, tasación, contacto, quiénes somos) sin depender de frameworks. |
| Versionado | Git y GitHub | Guardar el historial de cambios del proyecto, volver a versiones anteriores si algo falla y mantener el código respaldado en la nube. |
| Publicación | GitHub Pages | Publicar el sitio gratis con un enlace público para mostrarlo y probarlo en computador y celular. |
| Diseño | Whimsical | Armar el mapa del sitio, el flujo del usuario (Rodrigo Vega) y los wireframes de baja fidelidad antes de programar. |
| Diseño | Google Stitch | Generar propuestas visuales de las pantallas (inicio, ficha del auto) y explorar estilos antes de pasarlos a HTML y CSS. |
| IA | Claude | Generar ideas, textos del sitio, proto persona y funcionalidades; también revisar y depurar el código HTML y CSS. |
| Editor | Visual Studio Code | Escribir y revisar el código, con extensiones como Live Server para ver los cambios en el navegador al instante. |

## Qué es funcional y qué es prototipo

| Funcionalidad | Estado en esta versión |
| Catálogo de vehículos | Funcional (contenido estático) |
| Buscador y filtros | Prototipo visual |
| Ficha detallada del auto | Funcional (contenido estático) |
| Botón de WhatsApp | Funcional (enlace directo con mensaje prellenado) |
| Formulario de contacto y datos de la automotora | Prototipo visual (el mapa y los datos de contacto sí son funcionales) |
| Cotizador de financiamiento | Propotipo visual |
| Quiénes somos | Funcional (contenido estático) |
| Informe de inspección Fajardo | Prototipo visual (ejemplo con un auto) |
| Tasación en 24 h | Prototipo visual |
| Agenda de visita o test drive | Prototipo visual |
| Semáforo de confianza | Prototipo visual |
| Comparador de autos | Prototipo visual |
| Alertas personalizadas | Prototipo visual |

## Integraciones para una versión real

- WhatsApp Business: atención a clientes con mensajes automáticos y catálogo.
- Servicio de formularios (por ejemplo Formspree o Netlify Forms) o un backend propio: recibir los datos de contacto y tasación por correo.
- Base de datos de inventario o CMS: administrar autos, precios y fotos sin editar código.
- Google Maps: ubicación de la automotora y rutas.
- Calendario (Google Calendar o Calendly): agenda de visitas y test drive con confirmación automática.
- Financieras o bancos aliados: cotizador con tasas y condiciones reales.
- Servicios de verificación vehicular: consulta de prendas, multas e historial para el semáforo de confianza.
- Google Analytics: medir visitas, contactos y autos más vistos.

## Restricciones

- **Plazo: Por tiempo, la versión actual se limita a las funciones de prioridad alta, con el resto como prototipo visual.**
- **Marca: El sitio debe usar el nombre Fajardo Motors y transmitir confianza, transparencia y cercanía, coherente con la propuesta de valor (autos revisados, historial a la vista y garantía escrita).**
- **Dispositivos: Diseño responsive con enfoque móvil primero, ya que gran parte de los clientes llegará desde el celular o por WhatsApp. Se prueba además en computador y tablet.**
