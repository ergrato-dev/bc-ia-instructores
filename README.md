# bc-ia-instructores

> **Bootcamp corto · 2.5–3 horas**  
> IA en desarrollo de contenidos de formación  
> Dirigido a instructores ADSO — CGMLTI · SENA Bogotá

---

## ¿De qué trata este curso?

Una sesión práctica de capacitación entre pares donde exploramos cómo la inteligencia artificial generativa puede potenciar el trabajo de diseño instruccional, creación de materiales y gestión de contenidos de formación técnica.

No es un curso teórico sobre IA. Es una sesión de trabajo donde cada instructor sale con al menos **un artefacto real creado con IA** y un conjunto de prompts reutilizables para su área.

---

## Objetivos de aprendizaje

Al finalizar, cada participante podrá:

1. Explicar qué es la IA generativa y usarla con criterio ético en contextos de formación
2. Diseñar prompts efectivos para crear materiales pedagógicos (guías, rúbricas, RAP, GFPI)
3. Navegar la estructura de contenidos tipo bootcamp del repositorio `ergrato-dev`
4. Comprender qué hace Syllabot y cómo acceder a él
5. Distinguir entre chatbot, agente IA y pipeline automatizado
6. Entender qué es el protocolo MCP con ejemplos concretos

---

## Estructura del curso

| Módulo | Tema | Duración |
|--------|------|----------|
| M0 | Bienvenida y encuadre | 10 min |
| M1 | IA en formación: fundamentos y panorama | 30 min |
| M2 | Prompting para instructores | 45 min |
| M3 | Syllabot y repos `bc-` en GitHub | 35 min |
| M4 | Agentes IA y MCP | 40 min |
| M5 | Cierre, Q&A y próximos pasos | 20 min |
| **Total** | | **~3 horas** |

---

## Estructura del repositorio

```
bc-ia-instructores/
├── README.md                    ← este archivo
├── modulos/
│   ├── M0-bienvenida.md
│   ├── M1-fundamentos-ia.md
│   ├── M2-prompting.md
│   ├── M3-syllabot-repos.md
│   ├── M4-agentes-mcp.md
│   └── M5-cierre.md
├── talleres/
│   ├── T1-mejora-tu-prompt.md
│   ├── T2-rubrica-con-ia.md
│   └── T3-iteracion-colectiva.md
├── recursos/
│   ├── plantilla-prompt-sena.md
│   ├── prompts-ejemplo.md
│   ├── glosario.md
│   └── checklist-facilitador.md
└── assets/
    └── (imágenes y diagramas de apoyo)
```

---

## Cómo usar este repositorio

### Si eres participante del curso
1. No necesitas tener GitHub. Puedes leer todo directamente en esta página.
2. Los archivos en `/modulos` tienen el contenido de cada sesión.
3. Los archivos en `/talleres` tienen las actividades prácticas con instrucciones paso a paso.
4. En `/recursos` encuentras la plantilla de prompts y el glosario.

### Si eres facilitador
1. Lee primero `recursos/checklist-facilitador.md` — tiene todo lo que necesitas preparar.
2. Cada módulo en `/modulos` incluye **guía del instructor** y **material del participante** separados.
3. Los talleres en `/talleres` son autocontenidos: se pueden imprimir o proyectar.

---

## Herramientas referenciadas en el curso

| Herramienta | URL | Costo |
|-------------|-----|-------|
| Claude | [claude.ai](https://claude.ai) | Gratis / Pro |
| ChatGPT | [chatgpt.com](https://chatgpt.com) | Gratis / Plus |
| Gemini | [gemini.google.com](https://gemini.google.com) | Gratis |
| Perplexity | [perplexity.ai](https://perplexity.ai) | Gratis |
| GitHub Copilot | [github.com/features/copilot](https://github.com/features/copilot) | Pago |
| Syllabot | [syllabot.ergrato.dev](https://syllabot.ergrato.dev) | Interno SENA |
| Docs MCP | [modelcontextprotocol.io](https://modelcontextprotocol.io) | Gratis |

---

## Semilla: próximo curso — OpenClaw en VPS

> ⚠️ Este bloque es una vista previa. No hace parte del bootcamp actual.

**OpenClaw** ([openclaw.ai](https://openclaw.ai) · [github.com/openclaw/openclaw](https://github.com/openclaw/openclaw)) es un asistente IA personal de código abierto (MIT) que puedes instalar en tu propio servidor (VPS) y conectar a los canales que ya usas: WhatsApp, Telegram, Discord, Slack, entre otros.

### ¿Por qué importa para instructores?

| Sin OpenClaw | Con OpenClaw en VPS |
|---|---|
| Depende de cuentas gratuitas con límites | Tu propio asistente, sin tope de mensajes |
| Datos enviados a terceros | Datos en tu infraestructura |
| Un solo canal (web) | WhatsApp, Telegram, Discord, etc. |
| Sin personalización pedagógica | Skills propias con prompts SENA |

### ¿Qué cubriría el próximo curso?

1. Levantar un VPS Linux con Node 24
2. Instalar y configurar OpenClaw (`openclaw onboard`)
3. Conectar un canal (ej. Telegram)
4. Crear una *skill* personalizada para contexto SENA
5. Nociones de seguridad para producción

### Instalación básica (referencia)

```bash
# Instalar globalmente
pnpm add -g openclaw@latest

# Asistente de configuración interactivo
openclaw onboard --install-daemon
```

---

## Canal de referencia

📺 **BC Channel EPTI** — [@BCChannelEPTI](https://youtube.com/@BCChannelEPTI)  
Contenido técnico en español: Docker, Go, CI/CD, MCP, IA — enfocado en aprendices y desarrolladores hispanohablantes.

---

## Autor

**El Parche** · Instructor ADSO · CGMLTI · SENA Bogotá  
GitHub: [ergrato-dev](https://github.com/ergrato-dev)

---

> *Este repositorio es parte de la colección `bc-` de bootcamps del instructor.*  
> *Todo el material fue desarrollado con asistencia de IA y revisado por criterio docente humano.*
