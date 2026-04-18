---
applyTo: "modulos/**,talleres/**"
---

# Instrucciones: Módulos y Talleres

## Audiencia y nivel

- **Quién lee**: instructores ADSO del SENA con experiencia pedagógica — no aprendices
- **Nivel técnico**: intermedio/avanzado en pedagogía, básico/intermedio en IA
- **Sesión corta**: 2.5–3 horas totales, cada módulo debe caber en su tiempo estimado

## Idioma

- Documentación en **español**
- Términos técnicos de IA en **inglés**: prompt, token, RAG, MCP, pipeline, agent, LLM
- Terminología SENA en español: RAP, GFPI, ADSO, evidencias, competencia, aprendiz

## Estructura obligatoria de un módulo (`modulos/M{N}-*.md`)

```markdown
# M{N} · {Título}

> ⏱️ **{X} minutos** · {tipo de segmento}

## 🎯 Objetivo del módulo

## 👨‍🏫 Guía del facilitador

## 📋 Material del participante

## 🔗 Transición al siguiente módulo
```

## Estructura obligatoria de un taller (`talleres/T{N}-*.md`)

```markdown
# T{N} · {Título}

> ⏱️ **{X} minutos** · Materiales: {lista}

## 🎯 Objetivo

## 📋 Instrucciones (numeradas, paso a paso)

## ✅ Resultado esperado / entregable

## 🔁 Variantes opcionales
```

## Reglas de contenido

- ❌ No sobrecargar: si el contenido supera el tiempo estimado, dividir o recortar
- ✅ Incluir al menos un ejemplo concreto del contexto SENA (RAP, GFPI, rúbrica, guía)
- ✅ Los bloques de código o prompts deben ir en fences de código con lenguaje indicado
- ❌ No duplicar contenido del README; usar enlaces markdown a secciones existentes
- ✅ Al referenciar otro módulo o taller, usar enlace relativo: `[M2](../modulos/M2-prompting.md)`
