# M1 · IA en formación: fundamentos y panorama

> ⏱️ **30 minutos** · Módulo conceptual

---

## 🎯 Objetivo del módulo

Que cada participante tenga un modelo mental claro de qué es la IA generativa, qué herramientas existen, cuáles son los riesgos reales y cómo se relaciona esto con el trabajo de instructor en el SENA.

---

## 👨‍🏫 Guía del facilitador

### Talking points

#### 1. Qué es la IA generativa — sin rodeos (8 min)

No arrancar con una definición técnica. Arrancar con una analogía:

> "Imagínense un asistente que leyó una cantidad absurda de texto: libros, artículos, código, conversaciones, documentos académicos — básicamente todo el internet disponible hasta cierto punto. Ese asistente no 'sabe' cosas como nosotros: no tiene comprensión real. Pero es increíblemente bueno prediciendo qué palabra debería venir después de otra. Y resulta que eso, bien calibrado, produce texto que parece muy inteligente."

Puntos clave a enfatizar:

- **Genera, no busca**: no es Google. No va a buscar la respuesta correcta — va a generar una respuesta plausible.
- **Alucina**: puede inventar hechos, citas, referencias con total confianza. Esto no es un bug que van a arreglar pronto — es inherente al funcionamiento.
- **No recuerda**: cada conversación empieza de cero (salvo que el sistema tenga memoria explícita).
- **El modelo importa**: no todas las IAs son iguales. Claude, GPT-4, Gemini tienen capacidades y limitaciones diferentes.

**Pregunta detonadora**: "¿Alguien tiene un ejemplo de una vez que la IA les dio información incorrecta o rara?" — dejar que 1-2 personas cuenten.

---

#### 2. Herramientas clave — cuál usar para qué (7 min)

| Herramienta | Mejor para | Limitaciones |
|-------------|-----------|--------------|
| **Claude** (Anthropic) | Textos largos, documentos, razonamiento, código | Menos conocido en Colombia |
| **ChatGPT** (OpenAI) | Todo propósito, el más conocido | GPT-3.5 gratis es bastante limitado |
| **Gemini** (Google) | Integración con Google Workspace, búsqueda | Variable en calidad |
| **Perplexity** | Búsquedas con fuentes verificables | Solo búsqueda, no crea tanto |
| **Copilot** (GitHub/MS) | Código, autocompletado en VS Code | Requiere suscripción para lo bueno |

> **Recomendación práctica**: para trabajo de instructor, arranquen con Claude o ChatGPT Plus. Si no tienen presupuesto, la versión gratis de Claude o ChatGPT sirven para empezar, con limitaciones de uso diario.

---

#### 3. Riesgos reales en contexto SENA (8 min)

Estos son los riesgos que sí aplican a nuestro trabajo:

**Alucinaciones en contenido técnico**
> La IA puede generar código que parece correcto pero no funciona, o citar una norma SENA que no existe. Siempre verificar antes de usar con aprendices.

**Derechos de autor y propiedad intelectual**
> Si le piden a la IA que reproduzca un libro o una guía publicada, puede hacerlo. Eso es infracción. El material que generen con IA para SENA debe ser original o claramente referenciado.

**Datos de aprendices**
> **Nunca** ingresar nombres, documentos de identidad, notas, ni información personal de aprendices en ninguna IA pública. Esto viola la Ley 1581 de Habeas Data en Colombia.

**Dependencia sin criterio**
> El riesgo más silencioso: empezar a usar el output de la IA sin revisarlo. La IA puede producir guías de aprendizaje que suenan bien pero no están alineadas con el RAP real de la competencia.

**Cómo mitigarlos — regla simple**:
> "IA como borrador, criterio docente como revisión final."

---

#### 4. Oportunidades concretas para instructores (5 min)

Hacer esta lista colaborativa: preguntar al grupo "¿para qué creen que les podría servir?"
Complementar con:

- Generar el primer borrador de una guía de aprendizaje (y luego ajustar)
- Crear variaciones de ejercicios para diferentes niveles
- Redactar objetivos de aprendizaje alineados a competencias
- Generar preguntas de evaluación tipo SENA
- Crear rúbricas de evaluación de producto
- Traducir o adaptar contenido técnico en inglés
- Resumir documentos extensos (como resoluciones SENA)
- Generar ejemplos de código comentado para aprendices

---

### Pregunta difícil frecuente

**"¿La IA va a reemplazar a los instructores?"**

> Respuesta honesta: no en el horizonte inmediato, y menos en el SENA donde la evaluación de competencias requiere observación directa y criterio humano. Lo que sí va a pasar es que los instructores que sepan usar IA bien van a tener una ventaja real sobre los que no la usen. No es que la IA reemplaza al instructor — es que el instructor que usa IA reemplaza al que no la usa.

---

### Señales de tiempo

- 8 min: terminando qué es IA generativa, arrancando herramientas
- 18 min: terminando herramientas, arrancando riesgos
- 25 min: terminando riesgos, abriendo oportunidades
- 30 min: transición a M2

### Transición a M2

> "Perfecto. Ahora que tenemos el contexto, vamos a lo más útil del día: cómo hablarle bien a la IA para que nos dé lo que necesitamos. Esto se llama prompting y tiene técnica."

---

## 📋 Material del participante

### Qué es la IA generativa

La **IA generativa** es un tipo de inteligencia artificial entrenada con enormes volúmenes de texto, código e imágenes para aprender patrones y generar contenido nuevo.

No busca respuestas — las **genera** prediciendo qué debería decir dado un contexto.

**Lo que puede hacer bien:**
- Redactar, resumir, reformular texto
- Generar código funcional (con errores posibles)
- Responder preguntas sobre temas que conoce
- Seguir instrucciones complejas si están bien formuladas
- Mantener un rol o tono específico durante una conversación

**Lo que NO hace bien:**
- Acceder a información en tiempo real (salvo que tenga búsqueda web)
- Recordar conversaciones anteriores (por defecto)
- Garantizar que la información sea correcta
- Conocer documentos internos o privados que no le compartas

---

### Los 3 riesgos que más nos aplican

#### 🔴 Alucinaciones
La IA puede inventar hechos, citar normas que no existen o generar código que parece funcionar pero no funciona. **Siempre verificar antes de usar con aprendices.**

#### 🔴 Datos de aprendices
Nunca ingresar nombres, documentos, notas ni información personal de aprendices a ninguna IA pública. Ley 1581 — Habeas Data.

#### 🟡 Dependencia sin criterio
Usar el output de la IA sin revisarlo. El borrador de la IA es un punto de partida, no un producto final.

---

### Herramientas para empezar hoy

| Herramienta | Acceso | Mi recomendación |
|-------------|--------|-----------------|
| Claude | claude.ai | ⭐ Mejor para textos largos y documentos |
| ChatGPT | chatgpt.com | ⭐ Más conocido, gratis con límites |
| Gemini | gemini.google.com | Bien integrado con Google |
| Perplexity | perplexity.ai | Cuando necesito fuentes verificables |

---

### Mis notas del módulo

```
_____________________________________________
_____________________________________________
_____________________________________________
_____________________________________________
```
