# Publicación en GitHub Pages

**Archivo:** link en `README.md` · **Fase 3** · **4 pts**

## Qué es y para qué sirve

**Pasar a producción** es publicar el sitio para que cualquiera pueda visitarlo con una URL. **GitHub Pages** publica gratis los sitios HTML y CSS que están en un repositorio de GitHub.

Ya lo hiciste con tu portafolio en la evaluación anterior: es el mismo proceso.

## Qué entregas

- El sitio **publicado y accesible** en GitHub Pages.
- El **link** en la sección "Sitio publicado" del `README.md`.
- **Commits descriptivos** que muestren el avance de la implementación.

## Paso a paso

### 1. Revisa que la landing se llame `index.html`

GitHub Pages abre `index.html` por defecto. Debe estar en la **raíz** del repositorio, no dentro de una carpeta.

### 2. Sube todos los cambios

```bash
git add .
git commit -m "feat: completa implementación del sitio"
git push
```

### 3. Activa GitHub Pages

1. En tu repositorio, entra a **Settings → Pages**.
2. En **Source**, elige **Deploy from a branch**.
3. Elige la rama **main** y la carpeta **/ (root)**.
4. Guarda y espera unos minutos.

La URL queda así: `https://tu-usuario.github.io/mi-emprendimiento/` (o con el nombre que le hayas dado a tu fork).

### 4. Revisa el sitio publicado

Abre la URL **en una ventana de incógnito** y en tu **celular**. Recorre todas las páginas.

Los errores más comunes aparecen recién al publicar:

| Problema | Causa habitual | Solución |
|---|---|---|
| Página sin estilos | Ruta del CSS incorrecta | Usa rutas relativas: `css/styles.css`, no `/css/styles.css` ni `C:\...` |
| Imágenes rotas | Mayúsculas distintas (`Foto.PNG` vs `foto.png`) o tildes en el nombre | Nombres en minúsculas, sin espacios ni tildes, y escritos igual en el HTML |
| Error 404 al entrar | No hay `index.html` en la raíz | Mueve o renombra la landing |
| Cambios que no aparecen | GitHub Pages tarda unos minutos | Espera y recarga sin caché |

### 5. Agrega el link al README

```markdown
## Sitio publicado

https://tu-usuario.github.io/brote-jardineria/
```

Haz el último commit antes del **miércoles 14 de octubre a las 23:59**.

## Errores comunes

- **Publicar a última hora**: si algo falla, no alcanzas a corregirlo. Publica apenas tengas la landing y actualiza con cada avance.
- **Revisar solo en tu computador**: lo que funciona en local puede fallar publicado.
- **Olvidar el link en el README.**

## Checklist

- [ ] `index.html` en la raíz del repositorio
- [ ] GitHub Pages activado en la rama main
- [ ] Sitio revisado en incógnito y en el celular
- [ ] Sin páginas sin estilo ni imágenes rotas
- [ ] Link en el `README.md`
- [ ] Último commit antes del miércoles 14 de octubre, 23:59
