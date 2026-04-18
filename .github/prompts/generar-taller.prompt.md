---
mode: ask
description: Genera una actividad práctica (taller) para el bootcamp de instructores SENA
---

Genera el contenido completo del taller **T${input:taller_numero: número del taller (1-3)}** titulado **"${input:titulo: título del taller}"**.

## Datos del taller

- **Duración**: ${input:duracion: duración total, ej. 20 minutos}
- **Materiales**: ${input:materiales: qué necesita el participante, ej. "laptop, acceso a Claude o ChatGPT"}
- **Módulo relacionado**: ${input:modulo: módulo al que complementa, ej. "M2 - Prompting"}
- **Entregable esperado**: ${input:entregable: qué produce el participante, ej. "un prompt funcional para generar una rúbrica"}

## Contexto

- Audiencia: instructores ADSO con experiencia pedagógica, nivel básico/intermedio en IA
- El taller debe ser completable en el tiempo dado, individualmente o en parejas
- Usar ejemplos concretos del contexto SENA: RAP, GFPI, rúbricas, guías de aprendizaje, evidencias

## Estructura requerida

```
# T{N} · {Título}
> ⏱️ duración · Materiales: ...

## 🎯 Objetivo
(una sola frase con verbo de desempeño observable)

## 📋 Instrucciones
(numeradas, paso a paso, con tiempos aproximados por paso)

## ✅ Resultado esperado
(descripción del entregable + criterio de éxito mínimo)

## 🔁 Variantes opcionales
(para participantes avanzados o con más tiempo)
```

## Notas de diseño

- Las instrucciones deben ser autocontenidas: el participante no necesita al facilitador para ejecutarlas
- Incluir al menos 1 prompt de ejemplo como punto de partida (en bloque de código)
- El criterio de éxito debe ser observable, no subjetivo
