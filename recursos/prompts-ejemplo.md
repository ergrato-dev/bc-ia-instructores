# Banco de Prompts para Instructores ADSO · CGMLTI

> 10 prompts listos para copiar, pegar y ejecutar en Claude, ChatGPT o Gemini.
> Contexto: programa **ADSO · Centro CGMLTI · SENA Bogotá**.
> Para personalizar, reemplaza los valores entre corchetes `[...]`.

---

## Índice

| # | Tipo | Artefacto |
|---|------|-----------|
| 1 | Guía de aprendizaje | Guía de introducción a APIs REST |
| 2 | Guía de aprendizaje | Guía de fundamentos de bases de datos |
| 3 | Evaluación | Cuestionario diagnóstico de programación |
| 4 | Evaluación | Evaluación formativa de frontend |
| 5 | Rúbrica | Rúbrica de proyecto integrador (sistema web) |
| 6 | Rúbrica | Rúbrica de sustentación oral |
| 7 | GFPI | Cronograma trimestral de formación |
| 8 | GFPI | Actividades de aprendizaje para un RAP |
| 9 | GFPI | Evidencias de desempeño / producto / conocimiento |
| 10 | Transversal | Adaptación de material para aprendices con dificultades |

---

## Guías de aprendizaje

### Prompt 1 — Guía: introducción a APIs REST

```
Actúa como diseñador instruccional del SENA con dominio en desarrollo de
software y formación por proyectos.

Contexto: Programa ADSO, competencia "Construir los módulos del software
de acuerdo con el diseño y la arquitectura definidos", Centro CGMLTI Bogotá.
Aprendices en trimestre 3, fase lectiva. Conocen Python básico y HTML/CSS.
No han visto APIs REST antes.

Crea una guía de aprendizaje con:
- Título y objetivo de aprendizaje (redactado como RAP)
- Introducción: qué es una API REST y por qué la necesitan como desarrolladores
- Conceptos clave: recurso, endpoint, método HTTP (GET/POST/PUT/DELETE),
  código de respuesta, JSON
- Actividad 1 (conceptual): analizar una API pública sin código
- Actividad 2 (práctica): consumir una API pública con Python usando `requests`
- Actividad 3 (creación): diseñar los endpoints de una API simple en papel
  antes de codificar
- Recursos recomendados (documentación, herramientas)
- Criterios de evaluación básicos (verificables y observables)

Formato: Markdown con encabezados claros. Extensión: 500–700 palabras.
Tono: técnico y accesible, en español. No incluyas código fuente completo
en la guía — solo fragmentos ilustrativos cortos.
```

---

### Prompt 2 — Guía: fundamentos de bases de datos relacionales

```
Eres un instructor SENA especialista en bases de datos y diseño de sistemas
de información, con experiencia en ADSO.

Contexto: Competencia "Construir la solución de acuerdo con el diseño
previo, para el sistema de información", Centro CGMLTI, ficha en trimestre 2.
Aprendices tienen conocimientos de lógica de programación pero ninguna
experiencia previa en bases de datos.

Genera una guía de aprendizaje progresiva con:
- Objetivo (como RAP)
- Sección 1: ¿Qué es una base de datos relacional? (analogía con el mundo real)
- Sección 2: Entidades, atributos y relaciones — con un ejemplo del proyecto
  integrador de ADSO (sistema de gestión de fichas o de aprendices)
- Sección 3: Modelo Entidad-Relación — cómo leerlo e interpretarlo
- Sección 4: Normalización básica (1FN, 2FN, 3FN) con el mismo ejemplo
- Actividad práctica: modelar la base de datos de un caso sencillo dado
- Errores comunes en diseño de BD (lista de 5 antipatrones frecuentes)
- Criterios de evaluación

Formato: Markdown. Incluye tablas de ejemplo cuando sea útil.
Extensión: 600–800 palabras. Lenguaje: claro, español, sin anglicismos
innecesarios. Evita definiciones de diccionario — usa siempre el contexto
del proyecto integrador ADSO como ejemplo principal.
```

---

## Evaluaciones

### Prompt 3 — Evaluación diagnóstica de programación

```
Actúa como instructor evaluador del SENA con dominio en evaluación de
competencias técnicas en programación orientada a objetos.

Necesito una evaluación diagnóstica para medir el nivel de entrada de
aprendices nuevos al trimestre 3 del programa ADSO, que vienen del trimestre 2
con fundamentos de Python y lógica de programación.

Genera la evaluación con:
- 3 preguntas de selección múltiple sobre conceptos de POO (clase, objeto,
  herencia, encapsulamiento) — 4 opciones cada una, una sola correcta
- 2 preguntas de análisis de código: mostrar un fragmento Python y pedir
  que el aprendiz identifique qué hace o qué error tiene
- 1 ejercicio de diseño rápido: dado un caso del mundo real, identificar
  las clases, atributos y métodos principales (sin escribir código)

Para cada pregunta de selección múltiple: indicar respuesta correcta y
por qué las otras son incorrectas (para uso exclusivo del instructor).

Formato: Markdown. Dos secciones: "Versión aprendiz" (sin respuestas) y
"Guía del instructor" (con respuestas y justificaciones).
Tiempo estimado de aplicación: 20 minutos. Sin trampa — objetivo: diagnóstico
honesto del nivel real, no calificación.
```

---

### Prompt 4 — Evaluación formativa de frontend

```
Eres instructor del SENA con experiencia en desarrollo frontend y evaluación
formativa en el programa ADSO.

Contexto: Semana 6 del trimestre 3. Los aprendices llevan 3 semanas trabajando
con HTML5, CSS3 y JavaScript básico (DOM, eventos, fetch API).
Es evaluación formativa — retroalimentación, no nota final.

Diseña una evaluación formativa que incluya:
- 1 caso práctico breve: descripción de una pantalla de interfaz para el
  proyecto integrador (ejemplo: formulario de registro de aprendiz), con una
  imagen ASCII o descripción textual del layout esperado
- Tarea: el aprendiz debe codificar esa pantalla en 30 minutos con HTML + CSS
- Lista de verificación de criterios (checklist) que el instructor usa
  mientras observa al aprendiz trabajar (evaluación de desempeño)
- 3 preguntas de reflexión post-tarea para el aprendiz (autoevaluación)
- Escala de valoración: No alcanzado / En proceso / Alcanzado

Formato: Markdown. Lenguaje claro, descriptivo.
El caso práctico debe ser realista para el proyecto integrador de ADSO
(sistema de gestión escolar, tienda, o inventario — escoge el más adecuado).
```

---

## Rúbricas

### Prompt 5 — Rúbrica: proyecto integrador (sistema web)

```
Actúa como evaluador experto del SENA con dominio en rúbricas analíticas
y evaluación de proyectos de software en el programa ADSO.

El entregable a evaluar es:
- Sistema web de gestión [de inventario / académico / de ventas] desarrollado
  en equipo de 3 aprendices durante 8 semanas
- Stack: Python/FastAPI (o Django), PostgreSQL, HTML/CSS/JS, desplegado en
  servidor local o en la nube (Railway o Render)
- Debe incluir: CRUD completo, autenticación básica, interfaz funcional y
  documentación mínima

Genera una rúbrica analítica con:
- 5 criterios de evaluación:
  1. Funcionalidad (cumplimiento de requerimientos)
  2. Calidad del código (estructura, buenas prácticas, comentarios)
  3. Diseño de base de datos (normalización, integridad referencial)
  4. Interfaz de usuario (usabilidad, consistencia visual)
  5. Documentación y proceso (README, commits en GitHub, trabajo en equipo)
- 4 niveles: No alcanzado / En proceso / Alcanzado / Superado
- Descripción específica y observable para cada nivel de cada criterio
- Ponderación sugerida (suma 100%)
- Espacio para observaciones del evaluador

Formato: tabla Markdown. Criterios verificables sin ambigüedad.
No uses lenguaje subjetivo ("bonito", "bueno") — solo conductas observables.
```

---

### Prompt 6 — Rúbrica: sustentación oral de proyecto

```
Eres instructor del SENA con experiencia en evaluación de sustentaciones
técnicas y evidencias de conocimiento en el programa ADSO.

Necesito una rúbrica para evaluar la sustentación oral de 10 minutos que
cada aprendiz hace al final del trimestre sobre su proyecto integrador.
La sustentación incluye: presentación del problema, solución técnica
implementada, demostración en vivo del sistema y respuesta a preguntas.

Diseña la rúbrica con:
- 4 criterios:
  1. Dominio técnico del tema (explica cómo funciona lo que construyó)
  2. Claridad y estructura de la exposición (coherencia, tiempo, recursos)
  3. Demostración funcional (el sistema corre, muestra lo que prometió)
  4. Respuesta a preguntas (manejo de preguntas técnicas del jurado)
- 4 niveles: No alcanzado / En proceso / Alcanzado / Superado
- Indicadores observables para cada nivel de cada criterio
- Ponderación sugerida
- Campo de comentarios por criterio

Formato: tabla Markdown. Pensada para imprimirse y usarse en papel durante
la sustentación. Cada celda debe ser concisa (máx 2 líneas de texto).
```

---

## Instrumentos GFPI

### Prompt 7 — GFPI: cronograma trimestral

```
Actúa como coordinador académico del SENA con experiencia en planeación
del GFPI (Guía de Formación por Proyectos Integrador) y programación de
actividades de formación por competencias.

Situación:
- Programa: ADSO · Centro CGMLTI · Bogotá
- Trimestre: 4 de formación (de 6 totales del programa)
- Duración: 11 semanas de formación + 1 semana de cierre/evaluación
- Intensidad: 40 horas semanales (lunes a viernes, 8 horas/día)
- Proyecto integrador del trimestre: sistema de gestión académica

Competencias del trimestre:
1. "Construir los módulos del software de acuerdo con el diseño y la
   arquitectura definidos" (principal, 60% del tiempo)
2. "Implementar los esquemas de seguridad y control de acceso del sistema
   de información" (30% del tiempo)
3. "Validar el cumplimiento de los requerimientos del sistema de información"
   (10% — pruebas y evaluación final)

Genera un cronograma semanal con:
- Semana y fechas (desde 2025-01-13 al 2025-04-04)
- Competencia activa esa semana
- RAP o subtema principal
- Actividades de aprendizaje (3 por semana: teórica, práctica, proyecto)
- Entregable o evidencia de la semana
- Horas por competencia esa semana

Formato: tabla Markdown. La semana 12 es evaluación integral del proyecto.
Distribuye el trabajo para que el proyecto integrador sea demostrable
desde la semana 8 en adelante.
```

---

### Prompt 8 — GFPI: actividades de aprendizaje para un RAP

```
Eres diseñador instruccional del SENA con experiencia en redacción de
actividades de aprendizaje para el GFPI del programa ADSO.

RAP a trabajar:
"Desarrollar los módulos del sistema de información, aplicando el lenguaje
de programación, los patrones de diseño y las buenas prácticas de desarrollo,
de acuerdo con los requerimientos del proyecto."

Genera un conjunto de 6 actividades de aprendizaje progresivas para este RAP,
que cubran 3 semanas de formación (40 horas cada semana = 120 horas totales).

Para cada actividad incluye:
- Nombre de la actividad
- Tipo: conceptualización / experimentación / ejercitación / proyecto
- Duración estimada (en horas)
- Descripción detallada (qué hace el aprendiz, paso a paso)
- Recursos necesarios (herramientas, software, materiales)
- Producto o evidencia que genera la actividad
- Criterio de evaluación de esa actividad

Las actividades deben progresar de: analizar código existente →
entender patrones → aplicar en ejercicios guiados → implementar en el
proyecto integrador.

Formato: Markdown con encabezados por actividad. Lenguaje técnico y preciso.
```

---

### Prompt 9 — GFPI: evidencias por tipo (desempeño / producto / conocimiento)

```
Actúa como instructor evaluador del SENA con dominio en el diseño de
instrumentos de evaluación por competencias para el programa ADSO.

Competencia: "Implementar los esquemas de seguridad y control de acceso
del sistema de información, de acuerdo con los requerimientos del proyecto."

Necesito diseñar las evidencias de evaluación para esta competencia
siguiendo los tres tipos del modelo SENA:

1. EVIDENCIA DE CONOCIMIENTO: lo que el aprendiz sabe (conceptos, teoría)
2. EVIDENCIA DE DESEMPEÑO: lo que el aprendiz hace (proceso observable)
3. EVIDENCIA DE PRODUCTO: lo que el aprendiz entrega (artefacto tangible)

Para cada tipo genera:
- Nombre descriptivo de la evidencia
- Descripción de qué consiste
- Instrumento de evaluación sugerido (cuestionario / lista de verificación /
  rúbrica analítica)
- Criterios de evaluación específicos (mínimo 4 por evidencia)
- Ponderación sugerida dentro de la competencia (suma 100% entre los 3 tipos)

Las evidencias deben ser coherentes con el proyecto integrador de gestión
académica y verificables en el contexto del CGMLTI.
Formato: sección separada por tipo de evidencia, en Markdown.
```

---

## Transversal

### Prompt 10 — Adaptar material para aprendices con dificultades de aprendizaje

```
Eres instructor del SENA con formación en educación inclusiva y adaptación
de materiales pedagógicos para poblaciones diversas, en el programa ADSO.

Tengo el siguiente material (pega aquí el texto de la guía o actividad
que necesitas adaptar):

---
[PEGA AQUÍ EL MATERIAL ORIGINAL]
---

Este material está pensado para el nivel estándar del trimestre [X].
Necesito adaptarlo para un aprendiz que presenta:
[Selecciona lo que aplique:]
- Dificultades de comprensión lectora (textos largos)
- Dificultades con la abstracción matemática / lógica
- Bajo nivel previo de conocimientos tecnológicos
- Barrera de idioma (hispanohablante con nivel básico de lectura)

Genera una versión adaptada que:
- Simplifique el lenguaje sin perder el contenido técnico esencial
- Divida las instrucciones largas en pasos muy cortos (máx 2 líneas por paso)
- Añada un ejemplo concreto del entorno cotidiano antes de cada concepto
- Reemplace términos técnicos con explicaciones entre paréntesis la primera
  vez que aparecen
- Mantenga el mismo objetivo de aprendizaje y los mismos criterios de evaluación
- Indique con [APOYO ADICIONAL] los puntos donde el instructor debe
  acompañar de cerca

Formato: Markdown. Al inicio del documento, incluye una nota breve
(2 líneas) para el instructor explicando qué fue adaptado y por qué.
```

---

## Cómo iterar cuando el resultado no es el esperado

```
La respuesta anterior no cumple porque: [razón específica].
Por favor ajusta para que: [qué debe cambiar exactamente].
Mantén el resto igual.
```

```
Dame una variación del prompt anterior pero con enfoque más
[práctico / simplificado / técnico / detallado / corto].
```

```
El tono no es el adecuado — necesito algo más [formal / cercano /
directo]. Reescribe solo la introducción manteniendo el contenido.
```

---

> Ver también: [Plantilla base de prompt SENA](plantilla-prompt-sena.md) ·
> [Glosario de términos](glosario.md)
