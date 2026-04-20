# M3 · Repos `bc-` en GitHub

> ⏱️ **35 minutos** · Demo en vivo + exploración guiada

---

## 🎯 Objetivo del módulo

Que los participantes entiendan cómo está estructurado el modelo de contenidos tipo bootcamp del instructor anfitrión y cómo la IA apoya la creación y mantenimiento de esos contenidos en repositorios GitHub.

---

## 👨‍🏫 Guía del facilitador

### Estructura del módulo

| Segmento | Contenido | Tiempo |
|----------|-----------|--------|
| Contexto | Por qué estructurar contenidos en repos | 5 min |
| Tour repos | Navegar github.com/ergrato-dev en vivo | 15 min |
| IA + repos | Cómo la IA apoya el flujo completo | 15 min |

---

### Talking points

#### Por qué repos y no carpetas de Drive (5 min)

> "La mayoría usamos Google Drive o carpetas compartidas para nuestros materiales. Funciona, pero tiene problemas: no hay historial de cambios, no sabes qué versión es la actual, no puedes colaborar en tiempo real sin conflictos, y no hay forma de automatizar nada."

**Los repos de GitHub resuelven esto:**
- Historial completo de cambios (quién cambió qué y cuándo)
- Versiones claras por fecha o número de ficha
- Acceso público o privado según la necesidad
- Se pueden complementar con automatizaciones y pipelines

**La convención `bc-`:**
- Todos los repos de bootcamp siguen el prefijo `bc-`
- Ejemplo: `bc-docker`, `bc-go-fundamentos`, `bc-ia-instructores`
- Facilita identificarlos y filtrarlos en GitHub

---

#### Tour por ergrato-dev (15 min)

Abrir **https://github.com/ergrato-dev** en el navegador proyectado.

Mostrar en orden:
1. La lista de repos con prefijo `bc-`
2. Entrar a un repo de ejemplo
3. La estructura de carpetas (`modulos/`, `talleres/`, `recursos/`)
4. Cómo el `README.md` funciona como índice navegable
5. Cómo se ve en GitHub vs en VS Code local

**Punto clave:**
> "No necesitan saber Git para leer estos contenidos. GitHub los renderiza como páginas web. Cualquier persona puede acceder a la URL y navegar el curso completo sin instalar nada."

Invitar a 2–3 participantes a abrir el repo en su propio teléfono o computador y navegar por su cuenta 5 min.

---

#### IA + repos: el flujo completo (15 min)

Mostrar en vivo el flujo de principio a fin:

```
Prompt en Claude
      ↓
Contenido del módulo en Markdown
      ↓
Pegar en archivo del repo (VS Code)
      ↓
Commit y push a GitHub
      ↓
Aprendices leen en GitHub (sin instalar nada)
```

Demo rápida: tomar un output generado en el taller de M2 y mostrarlo "llegando" al repo.

---

### Transición a M4

> "Esto que acabamos de ver —donde la IA genera el contenido y lo publicamos directamente en GitHub para que cualquiera lo lea— es solo el primer paso. Ahora vamos a explorar qué pasa cuando la automatización es más sofisticada: los agentes IA."

---

## 📋 Material del participante

### Convención de repos `bc-`

```
bc-{tema}/
├── README.md           ← Índice y descripción del bootcamp
├── modulos/            ← Contenido de cada sesión
├── talleres/           ← Actividades prácticas
├── recursos/           ← Plantillas, glosario, referencias
└── assets/             ← Imágenes y archivos de apoyo
```

### El flujo IA → repo → aprendices

```
Claude genera Markdown → VS Code → GitHub → Aprendices
```

### Mis notas del módulo

```
_____________________________________________
_____________________________________________
_____________________________________________
```
