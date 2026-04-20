# 🤖 Instrucciones para GitHub Copilot

## 📋 Contexto del Proyecto

Este es el repositorio **bc-ia-instructores** — un bootcamp corto de 2.5–3 horas diseñado para instructores del programa ADSO (CGMLTI · SENA Bogotá). El objetivo es que cada instructor salga con al menos un artefacto real creado con IA y prompts reutilizables para su área.

- **Duración**: 2.5–3 horas (sesión única)
- **Audiencia**: Instructores ADSO — no aprendices
- **Formato**: Capacitación entre pares, hands-on
- **Repositorio padre**: colección `bc-` de [ergrato-dev](https://github.com/ergrato-dev)
- **README principal**: [README.md](../README.md)

---

## 🗂️ Estructura del Repositorio

```
bc-ia-instructores/
├── README.md                    ← entrada principal del repo
├── assets/
│   └── banner.svg               ← banner del encabezado
├── modulos/                     ← contenido por módulo (M0–M5)
│   ├── M0-bienvenida.md
│   ├── M1-fundamentos-ia.md
│   ├── M2-prompting.md
│   ├── M3-repos-bc.md
│   ├── M4-agentes-mcp.md
│   └── M5-cierre.md
├── talleres/                    ← actividades prácticas (T1–T3)
│   ├── T1-mejora-tu-prompt.md
│   ├── T2-rubrica-con-ia.md
│   └── T3-iteracion-colectiva.md
└── recursos/
    ├── checklist-facilitador.md
    ├── glosario.md
    └── plantilla-prompt-sena.md
```

### Nomenclatura de archivos

| Tipo         | Patrón           | Ejemplo                    |
| ------------ | ---------------- | -------------------------- |
| Módulo       | `M{N}-{slug}.md` | `M2-prompting.md`          |
| Taller       | `T{N}-{slug}.md` | `T1-mejora-tu-prompt.md`   |
| Recurso      | `{slug}.md`      | `checklist-facilitador.md` |
| Asset visual | `{slug}.svg`     | `banner.svg`               |

---

## 📝 Convenciones de Contenido

### Idioma

- **Documentación**: español
- **Código, slugs, nombres de archivos**: inglés o kebab-case en español cuando sea más claro para el público SENA
- **Términos técnicos**: inglés (prompt, token, MCP, agente, pipeline, etc.)

### Estructura de un módulo (`modulos/`)

Cada módulo debe incluir:

1. Título y descripción breve
2. Duración estimada
3. Objetivos del módulo
4. Contenido (con secciones claras)
5. Cierre / transición al siguiente módulo

### Estructura de un taller (`talleres/`)

Cada taller debe incluir:

1. Título, duración y materiales necesarios
2. Objetivo concreto
3. Instrucciones paso a paso numeradas
4. Resultado esperado / entregable
5. Variantes o extensiones opcionales

### Estructura de recursos (`recursos/`)

- `checklist-facilitador.md`: lista de verificación previa a la sesión
- `glosario.md`: términos clave ordenados alfabéticamente con definición concisa
- `plantilla-prompt-sena.md`: plantilla reutilizable con estructura de prompt para contexto SENA

---

## 🎨 Estándares de Diseño Visual

### Assets SVG (`assets/`)

- ✅ **Tema dark** — fondo `#0d1117` (GitHub dark)
- ✅ **Sin degradés** — cero `linearGradient` ni `radialGradient`
- ✅ **Fuentes sans-serif** — `system-ui`, `Arial`, `-apple-system` como fallback
- ❌ **Sin fuentes serif** (Times, Georgia, etc.)
- ✅ **Color de acento**: `#7B68EE` (Medium Slate Blue — color Peacock del proyecto)
- ✅ Preferir SVG sobre PNG/JPG para todos los gráficos y diagramas
- ✅ Texto alternativo descriptivo en markdown: `![Descripción](assets/nombre.svg)`

### Paleta de referencia

| Rol            | Hex       | Uso                               |
| -------------- | --------- | --------------------------------- |
| Background     | `#0d1117` | Fondo de banners y diagramas      |
| Surface        | `#161b22` | Superficies secundarias           |
| Accent         | `#7B68EE` | Líneas, bordes, nodos, highlights |
| Text primary   | `#ffffff` | Títulos                           |
| Text secondary | `#8b949e` | Subtítulos, descripciones         |
| Text muted     | `#3d444d` | Etiquetas, metadatos              |

---

## 🔀 Convenciones de Commits

Formato **Conventional Commits** en inglés con cuerpo pedagógico:

```
type(scope): short description

For: reason this change was needed
Impact: what this affects/enables
```

**Tipos**: `feat`, `fix`, `chore`, `docs`, `refactor`, `style`
**Scopes sugeridos**: `m0`–`m5`, `t1`–`t3`, `recursos`, `assets`, `readme`

**Ejemplos:**

```
docs(m2): add prompting techniques section

For: instructors need concrete examples for SENA use cases
Impact: covers RAP, GFPI and rubric generation patterns

feat(assets): add dark banner SVG for README header

For: visual identity consistent with bc- collection
Impact: improves repo presentation on GitHub
```

---

## 🤖 Instrucciones para Copilot

### Al generar contenido para módulos o talleres

1. **Mantén el nivel**: audiencia son instructores con experiencia pedagógica, no principiantes en tecnología
2. **Ejemplos concretos de SENA**: usar términos como RAP, GFPI, ADSO, evidencias de desempeño/producto/conocimiento
3. **Sesión corta**: el contenido debe poder leerse/ejecutarse en los tiempos indicados — no sobrecargar
4. **Formato markdown estándar**: encabezados `##` y `###`, listas, tablas y bloques de código

### Al generar assets SVG

- Aplicar la paleta dark definida arriba
- No usar `<defs><linearGradient>` ni `<radialGradient>`
- Tipografía: `font-family="-apple-system, BlinkMacSystemFont, 'Segoe UI', system-ui, Arial, sans-serif"`
- Dimensiones estándar para banners: `viewBox="0 0 1200 260"`

### Al dividir contenido largo

- Dividir por sección lógica (módulo, taller, recurso)
- Indicar qué parte se entrega y qué falta antes de continuar
- Esperar confirmación del usuario antes de la siguiente entrega

### Límites

- ❌ No crear archivos fuera de `modulos/`, `talleres/`, `recursos/` o `assets/`
- ❌ No agregar dependencias de npm/pnpm/pip — este repo es solo contenido Markdown + SVG
- ❌ No duplicar contenido que ya existe en el README; enlazar con markdown links

---

## 🔗 Recursos de Referencia

- [README principal](../README.md)
- [Checklist del facilitador](../recursos/checklist-facilitador.md)
- [Glosario](../recursos/glosario.md)
- [Repositorio de referencia bc-fastapi](https://github.com/ergrato-dev/bc-fastapi) — convenciones visuales y de commits
- [Docs MCP](https://modelcontextprotocol.io)
- [OpenClaw (próximo curso)](https://openclaw.ai)

---

_Proyecto: bc-ia-instructores · ergrato-dev · SENA Bogotá_
