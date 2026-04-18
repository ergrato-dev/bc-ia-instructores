# Plantilla de Prompt para Instructores SENA

> Archivo reutilizable · Adaptable a cualquier competencia del programa ADSO

---

## La plantilla base

Copia este bloque y completa cada sección entre corchetes:

```
[ROL]
Actúa como [diseñador instruccional / instructor experto en / especialista en]
con experiencia en [área técnica] y conocimiento del modelo pedagógico del SENA.

[CONTEXTO_SENA]
Estoy trabajando en el programa [ADSO / TIC / nombre del programa],
competencia: "[nombre exacto de la competencia]",
resultado de aprendizaje (RAP): "[texto del RAP si lo tienes]",
para aprendices de [CGMLTI / nombre del centro], ficha [número de ficha].
Los aprendices están en [fase lectiva / fase productiva] y tienen
[nivel básico / intermedio / avanzado] en el tema.

[TAREA]
Necesito que [generes / diseñes / crees / redactes]:
- [elemento 1]
- [elemento 2]
- [elemento 3]

[AUDIENCIA]
El material es para [aprendices del SENA de entre X y Y años /
instructores del centro / coordinadores académicos].
Su nivel previo en el tema es [ninguno / básico / intermedio].

[FORMATO]
Entrega el resultado en [Markdown / tabla / lista numerada / prosa].
[Incluye / No incluyes] [encabezados / ejemplos de código / tablas].
Extensión aproximada: [X párrafos / X palabras / X ítems].

[RESTRICCIONES]
- No uses [términos / herramientas / enfoques] que [razón]
- El lenguaje debe ser [formal / técnico / accesible] en español
- No incluyas [elementos no deseados]
- Basa el contenido en [fuentes / estándares] si es posible

[EJEMPLO_DE_SALIDA] (opcional pero muy útil)
Aquí un ejemplo del tipo de resultado que espero:
[pegar 2-3 líneas de ejemplo]
```

---

## Prompts de ejemplo listos para usar

### Prompt 1: Guía de aprendizaje

```
Actúa como diseñador instruccional especializado en formación técnica del SENA,
con dominio del enfoque de formación por proyectos y competencias laborales.

Estoy en el programa ADSO (Análisis y Desarrollo de Software), trabajando la
competencia técnica: "Construir los módulos del software, de acuerdo con el
diseño y la arquitectura definidos", para aprendices del CGMLTI en Bogotá.
Los aprendices tienen conocimientos básicos de programación en Python.

Crea el borrador de una guía de aprendizaje con esta estructura:
- Introducción (qué aprenderá el aprendiz y por qué es relevante)
- Objetivo de aprendizaje (redactado como RAP)
- Actividades de aprendizaje (3 actividades, progresivas en dificultad)
- Recursos requeridos (herramientas, software, referencias)
- Criterios de evaluación básicos

El material es para aprendices entre 18 y 25 años, nivel básico-intermedio.
Usa Markdown con encabezados claros. Extensión: entre 400 y 600 palabras.
No incluyas código fuente en la guía — solo la estructura pedagógica.
El tono debe ser técnico pero accesible, en español colombiano.
```

---

### Prompt 2: Evaluación de conocimientos

```
Eres un instructor SENA experto en evaluación de competencias técnicas en
el programa ADSO, con dominio de los tipos de evaluación del SENA
(diagnóstica, formativa, sumativa).

Necesito crear una evaluación de conocimientos sobre el tema:
"Fundamentos de bases de datos relacionales: modelo entidad-relación y
normalización hasta tercera forma normal".

Genera una evaluación con:
- 5 preguntas de selección múltiple con única respuesta (4 opciones A/B/C/D)
- 2 preguntas de verdadero/falso con justificación breve
- 1 pregunta de análisis corto (máx 5 líneas de respuesta)

Para cada pregunta de selección múltiple, indica al final cuál es la respuesta
correcta y una breve justificación (2-3 líneas) de por qué las otras opciones
son incorrectas.

Audiencia: aprendices del trimestre 3 del programa ADSO, con 2 meses de
formación en bases de datos. Nivel: básico-intermedio.
Formato: Markdown. Numeración clara. Sin ambigüedades en las preguntas.
Evita preguntas trampa — el objetivo es evaluar comprensión, no confundir.
```

---

### Prompt 3: Rúbrica de evaluación de producto

```
Actúa como evaluador experto en competencias técnicas del SENA, con
conocimiento de los instrumentos de evaluación del SGDEA.

Necesito diseñar una rúbrica de evaluación de producto para el siguiente
entregable de proyecto integrador:
"Sistema web de gestión de inventario desarrollado en equipo de 3 aprendices,
usando Python/Django, PostgreSQL y desplegado en un servidor local".

La rúbrica debe evaluar:
- Funcionalidad del sistema (qué tan completo es)
- Calidad del código (organización, comentarios, buenas prácticas)
- Documentación técnica (README, manual de usuario básico)
- Trabajo en equipo y proceso (evidencias de colaboración en GitHub)

Formato de la rúbrica:
- 4 criterios de evaluación
- 4 niveles de desempeño: No alcanzado / En proceso / Alcanzado / Superado
- Descripción clara de cada nivel para cada criterio
- Ponderación sugerida para cada criterio (debe sumar 100%)

Presenta la rúbrica como tabla Markdown. Lenguaje claro, sin ambigüedades.
Los criterios deben ser verificables y observables, no subjetivos.
```

---

### Prompt 4: Redacción de RAP

```
Eres un experto en diseño curricular del SENA con dominio de la metodología
de normalización de competencias y redacción de resultados de aprendizaje (RAP).

Tengo la siguiente competencia del programa ADSO:
"Implementar los esquemas de seguridad y control de acceso del sistema
de información, de acuerdo con los requerimientos del proyecto"

Necesito que generes 3 RAPs para esta competencia siguiendo el formato estándar
del SENA:
"[Verbo en infinitivo] [objeto directo] [condición de calidad / criterio]
de acuerdo con [estándar / requerimiento / metodología]"

Ejemplos del formato esperado:
- "Desarrollar la interfaz de usuario del sistema de información, aplicando
  estándares de usabilidad, de acuerdo con los requerimientos del proyecto."
- "Implementar las funcionalidades del sistema de información, según el diseño
  técnico y los requerimientos funcionales establecidos."

Los RAPs deben ser:
- Redactados en tercera persona del singular (el aprendiz...)
- Verificables y evaluables
- Coherentes con el contexto tecnológico actual (2024-2025)
- Apropiados para el nivel técnico del programa ADSO
```

---

### Prompt 5: Cronograma de formación (GFPI)

```
Actúa como coordinador académico del SENA con experiencia en planeación
pedagógica y diligenciamiento del GFPI (Guía de Formación por Proyectos
Integrador).

Necesito crear un cronograma de formación para la siguiente situación:
- Programa: ADSO (Análisis y Desarrollo de Software)
- Centro: CGMLTI, Bogotá
- Ficha: trimestre 4 de formación
- Duración: 12 semanas (3 meses)
- Intensidad: 40 horas semanales
- Proyecto integrador: "Sistema de gestión académica para una institución educativa"

Competencias a trabajar en este trimestre:
1. Construir los módulos del software según diseño y arquitectura definidos
2. Implementar esquemas de seguridad y control de acceso
3. Realizar pruebas de software de acuerdo con los requerimientos del proyecto

Genera un cronograma semanal que incluya:
- Semana (número y fechas aproximadas)
- Competencia y RAP principal de la semana
- Actividades de aprendizaje principales
- Entregable o evidencia de la semana

Formato: tabla Markdown con columnas: Semana | Fechas | Competencia/RAP |
Actividades principales | Entregable.

Distribuye las horas de forma coherente. En las últimas 2 semanas incluye
tiempo de consolidación y evaluación final del proyecto.
```

---

## Cómo iterar un prompt que no dio el resultado esperado

Cuando la respuesta no es lo que esperabas, no empieces de cero. Dile a la IA:

```
La respuesta anterior no cumple porque: [razón específica].
Por favor ajusta para que: [qué debe cambiar].
Mantén el resto igual.
```

O si quieres una versión diferente:

```
Dame una variación de lo anterior pero con un enfoque más [práctico / técnico /
simplificado / detallado].
```

---

> *Esta plantilla fue creada con asistencia de IA y revisada por criterio docente.*
> *Última actualización: 2025*
