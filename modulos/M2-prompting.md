# M2 · Prompting para instructores

> ⏱️ **45 minutos** · Módulo técnico + taller práctico

---

## 🎯 Objetivo del módulo

Que cada participante comprenda y aplique al menos 2 técnicas de prompting para crear materiales de formación, y salga con un artefacto real generado durante el taller.

---

## 👨‍🏫 Guía del facilitador

### Estructura del módulo

| Segmento | Contenido | Tiempo |
|----------|-----------|--------|
| Conceptual | Anatomía de un prompt + 4 técnicas | 20 min |
| Demo | El facilitador genera en vivo un ejemplo | 5 min |
| Taller | 3 ejercicios escalonados | 20 min |

---

### Talking points

#### Anatomía de un buen prompt (5 min)

Mostrar en vivo. Abrir Claude o ChatGPT y escribir dos prompts para lo mismo:

**Prompt malo:**
```
Hazme una guía de aprendizaje de Python
```

**Prompt bueno:**
```
Actúa como diseñador instruccional del SENA especializado en programación.
Crea el borrador de una guía de aprendizaje para la competencia técnica
"Desarrollar módulos de software con técnicas de programación" del programa ADSO.

La guía debe incluir:
- Objetivo de aprendizaje (redactado en términos de RAP)
- Actividades de aprendizaje (3 actividades, nivel básico)
- Recursos requeridos
- Criterios de evaluación básicos

Audiencia: aprendices del SENA, nivel técnico, entre 18 y 25 años.
Formato: Markdown, con encabezados claros.
No incluyas código en esta guía — solo la estructura pedagógica.
```

Mostrar la diferencia de output en vivo. Esto solo toma 2 minutos y es el mejor argumento.

**Las 6 partes de un prompt efectivo:**

1. **ROL** — quién es la IA en esta conversación
2. **CONTEXTO** — qué sabe la IA sobre la situación
3. **TAREA** — qué tiene que hacer exactamente
4. **AUDIENCIA** — para quién es el output
5. **FORMATO** — cómo quiero recibir la respuesta
6. **RESTRICCIONES** — qué NO debe hacer

---

#### Las 4 técnicas de prompting (15 min)

##### Técnica 1: Zero-Shot Prompting (3 min)

Le pides algo a la IA sin darle ejemplos. Funciona para tareas comunes y bien definidas.

**Ejemplo aplicado:**
```
Eres un instructor SENA experto en bases de datos.
Crea 5 preguntas de selección múltiple sobre normalización de bases de datos
para evaluar aprendices del programa ADSO al nivel de la RAP:
"Diseñar la estructura de datos requerida en el sistema de información".
Las preguntas deben tener 4 opciones cada una (A, B, C, D) con una sola
respuesta correcta. Incluye la respuesta correcta al final de cada pregunta.
```

**Cuándo usarlo:** tareas claras, cuando sabes exactamente qué quieres.
**Limitación:** si la tarea es compleja o ambigua, la respuesta puede ser genérica.

---

##### Técnica 2: Few-Shot Prompting (4 min)

Le das a la IA 2-3 ejemplos de lo que quieres ANTES de pedirle que genere.

**Ejemplo aplicado:**
```
Voy a darte ejemplos de cómo redacto resultados de aprendizaje (RAP)
en el SENA, y luego quiero que generes 3 más para la competencia indicada.

EJEMPLOS:
RAP 1: "Desarrollar la interfaz de usuario del sistema de información,
aplicando estándares de usabilidad, de acuerdo con los requerimientos
del proyecto."

RAP 2: "Implementar las funcionalidades del sistema de información,
según el diseño técnico y los requerimientos funcionales establecidos."

COMPETENCIA OBJETIVO:
"Implementar los esquemas de seguridad y control del sistema de información"

Genera 3 RAPs para esta competencia siguiendo el mismo estilo y estructura
de los ejemplos anteriores.
```

**Cuándo usarlo:** cuando tienes formato o estilo específico que quieres replicar.
**Ventaja clave:** la IA aprende el patrón de tus ejemplos, no de su entrenamiento general.

---

##### Técnica 3: Chain-of-Thought — CoT (4 min)

Le pides a la IA que "piense en voz alta" antes de dar la respuesta. Útil para tareas complejas.

**Ejemplo aplicado:**
```
Necesito diseñar un instrumento de evaluación para la competencia
"Construir soluciones de software en el marco del desarrollo ágil".

Antes de generar el instrumento, analiza paso a paso:
1. ¿Cuáles son los saberes clave de esta competencia (saber, saber hacer, ser)?
2. ¿Qué evidencias de desempeño son más relevantes para evaluar?
3. ¿Qué técnicas e instrumentos de evaluación son más apropiados para el SENA?

Con base en ese análisis, diseña el instrumento de evaluación.
```

**Por qué funciona:** forzar a la IA a razonar antes de responder reduce errores y produce outputs más coherentes.
**Variante útil:** añadir `"Primero, describe tu plan. Luego, ejecuta el plan."` a cualquier prompt complejo.

---

##### Técnica 4: Role Prompting (4 min)

Darle un rol específico a la IA cambia su "perspectiva" y el tono de sus respuestas.

**Ejemplo básico:**
```
Actúa como un instructor SENA con 15 años de experiencia en el programa ADSO,
especializado en programación orientada a objetos con Java.
Tu estilo de enseñanza es práctico y directo: siempre explicas con ejemplos
reales antes de dar la teoría.
```

**Combinado con CoT:**
```
Eres un diseñador instruccional experto en formación por proyectos (metodología SENA).
Un instructor te consulta: "Quiero que mis aprendices desarrollen un sistema de
inventario como proyecto integrador del trimestre. ¿Cómo lo estructuro?"

Piensa primero en las fases del proyecto, los entregables por fase,
cómo alinearlos a las RAPs del programa, y qué criterios de evaluación aplicarías.
Luego presenta tu propuesta de forma clara y accionable.
```

---

#### Demo en vivo — 5 min

El facilitador genera en tiempo real una rúbrica de evaluación usando la plantilla de prompt.
Proyectar la pantalla. Mostrar el prompt, la respuesta y una iteración rápida.

---

### Señales de tiempo

- 20 min: terminando las 4 técnicas, arrancando la demo
- 25 min: arrancando taller
- 45 min: cierre del taller, transición a M3

### Transición a M3

> "Muy bien. Ahora les voy a mostrar cómo yo organizo estos contenidos que generamos —ya sea con IA o sin ella— en repositorios de GitHub para que cualquier aprendiz pueda acceder a ellos directamente."

---

## 📋 Material del participante

### Las 6 partes de un prompt efectivo

```
[ROL]          → Quién es la IA en esta conversación
[CONTEXTO]     → Qué información relevante necesita saber
[TAREA]        → Qué tiene que hacer exactamente
[AUDIENCIA]    → Para quién es el output
[FORMATO]      → Cómo quiero recibir la respuesta
[RESTRICCIONES] → Qué NO debe hacer o incluir
```

### Comparación de técnicas

| Técnica | Cuándo usarla | Complejidad |
|---------|--------------|-------------|
| Zero-Shot | Tarea clara y bien definida | ⭐ Baja |
| Few-Shot | Necesito replicar un estilo o formato | ⭐⭐ Media |
| Chain-of-Thought | Tarea compleja, necesito razonamiento | ⭐⭐ Media |
| Role Prompting | Quiero un tono o perspectiva específica | ⭐ Baja |
| Combinadas | Tareas complejas y de alto valor | ⭐⭐⭐ Alta |

### Regla de oro del prompting

> **Si el output de la IA no es lo que esperabas, el problema casi siempre está en tu prompt, no en la IA.**

Las 3 causas más comunes de un prompt malo:
1. Contexto insuficiente — la IA no sabe quién eres ni para qué es esto
2. Tarea ambigua — "hazme algo sobre X" en vez de "genera exactamente Y"
3. Sin restricciones — no le dijiste qué NO quieres

---

## 🔗 Ver también

- [`talleres/T1-mejora-tu-prompt.md`](../talleres/T1-mejora-tu-prompt.md)
- [`talleres/T2-rubrica-con-ia.md`](../talleres/T2-rubrica-con-ia.md)
- [`talleres/T3-iteracion-colectiva.md`](../talleres/T3-iteracion-colectiva.md)
- [`recursos/plantilla-prompt-sena.md`](../recursos/plantilla-prompt-sena.md)
- [`recursos/prompts-ejemplo.md`](../recursos/prompts-ejemplo.md)
