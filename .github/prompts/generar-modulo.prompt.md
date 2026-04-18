---
mode: ask
description: Genera el contenido completo de un módulo del bootcamp para instructores SENA
---

Genera el contenido completo del módulo **${input:modulo_numero: número del módulo (0-5)}** titulado **"${input:titulo: título del módulo}"** para el bootcamp bc-ia-instructores.

## Datos del módulo

- **Duración**: ${input:duracion: duración estimada, ej. 30 minutos}
- **Posición**: ${input:posicion: qué módulo viene antes y después, ej. "después de M1, antes de M3"}
- **Objetivo central**: ${input:objetivo: en una frase, qué debe lograr el instructor al terminar}

## Contexto del proyecto

Este es un bootcamp de **2.5–3 horas** para instructores ADSO del SENA (no aprendices). La audiencia tiene experiencia pedagógica pero nivel básico/intermedio en IA. Cada instructor debe salir con al menos un artefacto real.

- Usa terminología SENA cuando sea relevante: RAP, GFPI, evidencias, competencia, ficha
- Los ejemplos de prompts deben ser accionables en Claude, ChatGPT o Gemini
- El tono es entre pares: directo, práctico, sin condescendencia

## Estructura requerida

Sigue exactamente la estructura definida en [content-modulos-talleres.instructions.md](../instructions/content-modulos-talleres.instructions.md):

```
# M{N} · {Título}
> ⏱️ duración

## 🎯 Objetivo del módulo
## 👨‍🏫 Guía del facilitador
   - Talking points con tiempos
   - Al menos 1 demo o ejemplo en vivo
## 📋 Material del participante
   - Contenido que el participante puede leer/usar
## 🔗 Transición al siguiente módulo
```

## Entrega

Genera el archivo completo en Markdown. Si el contenido es extenso, entrégalo por secciones e indica cuándo continuar.
