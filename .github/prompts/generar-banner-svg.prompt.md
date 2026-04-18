---
mode: ask
description: Genera un banner SVG dark para encabezados de módulos, talleres o recursos del bootcamp
---

Genera un banner SVG para **${input:destino: dónde va el banner, ej. "M2 - Prompting" o "T1 - Mejora tu prompt"}**.

## Datos del banner

- **Título principal**: ${input:titulo: texto principal, ej. "M2 · Prompting"}
- **Subtítulo**: ${input:subtitulo: texto secundario, ej. "Técnicas para instructores SENA"}
- **Etiqueta inferior** (opcional): ${input:etiqueta: texto muy pequeño, ej. "45 min · Módulo técnico"}

## Reglas de diseño (obligatorias)

Sigue las reglas definidas en [assets-svg.instructions.md](../instructions/assets-svg.instructions.md):

- ✅ Fondo: `#0d1117`
- ✅ Acento: `#7B68EE`
- ✅ Barra superior de 3px en `#7B68EE`
- ✅ Fuente: `-apple-system, BlinkMacSystemFont, 'Segoe UI', system-ui, Arial, sans-serif`
- ❌ Sin `linearGradient` ni `radialGradient`
- ❌ Sin fuentes serif
- `viewBox="0 0 1200 260"`

## Elementos decorativos sugeridos

Usa uno de estos patrones a los costados del texto:

- **Nodos de circuito**: líneas + círculos stroke en `#7B68EE` con opacidad baja
- **Dot grid**: `<pattern>` con puntos al 5% de opacidad
- **Líneas geométricas**: formas angulares simples

## Entrega

Devuelve el SVG completo listo para guardar en `assets/${input:nombre_archivo: nombre del archivo sin extensión, ej. "banner-m2-prompting"}.svg` y el snippet markdown para incluirlo:

```markdown
![{titulo}](assets/{nombre_archivo}.svg)
```
