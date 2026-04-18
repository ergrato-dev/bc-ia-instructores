---
applyTo: "assets/**"
---

# Instrucciones: Assets SVG

## Reglas absolutas (sin excepciones)

- ❌ **Cero degradés**: prohibido `<linearGradient>`, `<radialGradient>`, `<meshGradient>`
- ❌ **Cero fuentes serif**: prohibido Times, Georgia, Palatino, serif genérico
- ✅ **Solo colores sólidos** con `fill-opacity` para transparencias sutiles
- ✅ **Tema dark siempre**: fondo `#0d1117`, nunca blanco ni gris claro

## Paleta obligatoria

| Variable conceptual | Hex       | Uso concreto                             |
| ------------------- | --------- | ---------------------------------------- |
| Background          | `#0d1117` | `<rect>` de fondo principal              |
| Surface             | `#161b22` | Tarjetas, cajas, superficies secundarias |
| Accent              | `#7B68EE` | Líneas, bordes, nodos, barras destacadas |
| Text primary        | `#ffffff` | Títulos `<text>` principales             |
| Text secondary      | `#8b949e` | Subtítulos, descripciones                |
| Text muted          | `#3d444d` | Etiquetas, metadatos, fechas             |

## Tipografía

```svg
font-family="-apple-system, BlinkMacSystemFont, 'Segoe UI', system-ui, Arial, sans-serif"
```

- Títulos: `font-weight="700"`, `font-size="48"–"60"`
- Subtítulos: `font-weight="400"`, `font-size="16"–"20"`
- Etiquetas: `font-weight="400"`, `font-size="11"–"13"`, `letter-spacing="2"–"4"`

## Dimensiones estándar

| Tipo      | `viewBox`      | Uso                  |
| --------- | -------------- | -------------------- |
| Banner    | `0 0 1200 260` | Encabezado de README |
| Diagrama  | `0 0 800 500`  | Diagramas en módulos |
| Miniatura | `0 0 400 200`  | Tarjetas o previews  |

## Barra de acento superior (patrón de identidad)

Todo banner debe abrir con:

```svg
<!-- Barra de identidad bc- collection -->
<rect width="1200" height="3" fill="#7B68EE"/>
```

## Patrones decorativos permitidos

- Dot grid con `<pattern>` + `<circle>` de baja opacidad (`fill-opacity="0.05"`)
- Nodos de circuito: líneas `stroke="#7B68EE"` + círculos con `fill="#0d1117"` y stroke accent
- Líneas geométricas simples

## Vincular en markdown

```markdown
![Descripción del asset](assets/nombre-del-archivo.svg)
```

Siempre incluir texto alternativo descriptivo.
