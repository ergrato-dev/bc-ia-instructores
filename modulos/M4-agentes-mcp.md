# M4 · Agentes IA y MCP

> ⏱️ **40 minutos** · Conceptual + demo

---

## 🎯 Objetivo del módulo

Que los participantes distingan entre chatbot y agente IA, entiendan qué problema resuelve el protocolo MCP y vean en vivo un ejemplo de cómo estos conceptos aplican en contextos reales de formación.

---

## 👨‍🏫 Guía del facilitador

### Estructura del módulo

| Segmento | Contenido | Tiempo |
|----------|-----------|--------|
| Concepto | Chatbot vs agente vs pipeline | 10 min |
| MCP | Qué es y para qué sirve | 10 min |
| Demo | Agente con acceso a GitHub | 10 min |
| Posibilidades | Qué podríamos hacer en CGMLTI | 10 min |

---

### Talking points

#### Chatbot vs Agente IA (10 min)

**Analogía del aprendiz:**

> "Un chatbot es como un aprendiz muy listo que solo puede hablar. Puede responderme preguntas, redactar textos, explicar conceptos. Pero si le digo 'busca en mi Drive los syllabus del trimestre anterior y compáralos con los nuevos', se queda sin poder hacer nada — solo sabe hablar."

> "Un agente IA es ese mismo aprendiz, pero ahora tiene manos: puede abrir el computador, buscar en Drive, leer archivos, escribir en un documento. Puede *hacer* cosas, no solo *decir* cosas."

**Diferencia técnica simple:**

| Capacidad | Chatbot | Agente IA |
|-----------|---------|-----------|
| Genera texto | ✅ | ✅ |
| Accede a sistemas externos | ❌ | ✅ |
| Ejecuta acciones | ❌ | ✅ |
| Encadena pasos autónomamente | ❌ | ✅ |
| Ejemplos | ChatGPT básico | Claude + herramientas, Claude Code |

**Ejemplos útiles para instructores:**
- Agente que lee un repo GitHub y genera el sílabo para la ficha
- Agente que revisa el código de un aprendiz contra los criterios de la rúbrica
- Agente que busca referencias actualizadas y las agrega al material del módulo

---

#### Model Context Protocol — MCP (10 min)

> "Cuando decimos que un agente puede 'acceder a sistemas externos', eso no es magia. Alguien tiene que definir cómo se conecta. Ahí es donde entra MCP."

**Analogía del enchufe universal:**
> "MCP es como un estándar de enchufes. Antes, cada herramienta tenía su propio conector y necesitabas una integración personalizada para cada una. MCP define un protocolo estándar para que cualquier herramienta pueda conectarse con cualquier IA de la misma forma."

**Qué resuelve:**
- Los LLMs por defecto no pueden acceder a nada externo
- MCP define cómo un servidor de herramientas le dice a la IA qué puede hacer
- La IA decide cuándo y cómo usar cada herramienta durante la conversación

**Servidores MCP ya disponibles:**

| Servidor | Qué permite |
|----------|-------------|
| GitHub MCP | Leer y escribir repositorios |
| Google Drive MCP | Acceder a documentos de Drive |
| PostgreSQL MCP | Consultar bases de datos |
| Filesystem MCP | Leer y escribir archivos locales |

**Referencia:** [modelcontextprotocol.io](https://modelcontextprotocol.io)

---

#### Demo: agente + MCP en acción (10 min)

**Opción A — conexión estable:**
Mostrar Claude Code leyendo el repo `bc-ia-instructores` y generando automáticamente el contenido de un módulo nuevo en Markdown.

**Opción B — demo simplificada:**
Mostrar Claude.ai con búsqueda web habilitada: buscar recursos actualizados sobre un tema técnico y generar el material de referencia de un módulo.

**Punto clave:**
> "Lo que acaban de ver no requiere saber programar para usarlo. Las interfaces como Claude.ai ya abstraen toda la complejidad de MCP. El estándar es técnico, pero el uso es accesible."

---

#### Posibilidades para CGMLTI (10 min)

**Pregunta detonadora al grupo:**
> "¿Qué tarea de su trabajo como instructores les consume más tiempo pero es repetitiva?"

Mapear en el tablero. Luego mostrar la tabla de posibilidades:

| Tarea repetitiva | Agente posible |
|-----------------|---------------|
| Crear guías de aprendizaje | Agente con acceso al plan de estudios ADSO |
| Generar evaluaciones | Agente con banco de preguntas por competencia |
| Seguimiento de aprendices | SICORA (sistema del CGMLTI, en desarrollo) |
| Actualizar materiales | Agente que detecta cambios en tecnologías relevantes |

---

### Preguntas difíciles frecuentes

**"¿Cuánto cuesta implementar un agente para el centro?"**
> Depende de la complejidad. Un agente simple usando APIs de Claude cuesta centavos de dólar por consulta. Lo más costoso es el tiempo de desarrollo — que es donde tiene sentido usar Claude Code.

**"¿Necesito saber programar para usar MCP?"**
> Para usar agentes como usuario: no. Para construir un servidor MCP propio: sí, pero no es tan complejo. Hay servidores MCP open source para los casos de uso más comunes.

---

### Transición a M5

> "Estamos llegando al final. Quiero que tengamos un espacio para preguntas reales y para definir qué se llevan de acá y qué viene después."

---

## 📋 Material del participante

### Chatbot vs Agente IA

Un **chatbot** conversa.
Un **agente IA** conversa Y actúa.

La diferencia está en el acceso a herramientas externas y la capacidad de ejecutar acciones.

### Qué es MCP

**Model Context Protocol** — estándar abierto (Anthropic, 2024) que define cómo los modelos de lenguaje se conectan con herramientas y fuentes de datos externas.

- Docs: [modelcontextprotocol.io](https://modelcontextprotocol.io)
- Video explicativo: [@BCChannelEPTI](https://youtube.com/@BCChannelEPTI)

### Mis ideas para CGMLTI

```
_____________________________________________
_____________________________________________
_____________________________________________
```
