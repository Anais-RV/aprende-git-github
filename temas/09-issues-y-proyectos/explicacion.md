# Issues y Proyectos de GitHub

## ¿Qué es un Issue?

Un **Issue** es una forma de registrar una tarea, un error, una pregunta o una mejora pendiente en un repositorio de GitHub. Funciona como un sistema de tickets integrado directamente con el código.

Úsalos para:
- Reportar un error: "La función de login falla cuando el email tiene mayúsculas"
- Proponer una mejora: "Sería útil añadir un modo oscuro"
- Hacer una pregunta: "¿Cuál es la forma recomendada de configurar X?"
- Planificar trabajo: "Añadir validación al formulario de registro"

---

## Anatomía de un buen Issue

Un Issue útil incluye:

- **Título claro**: describe el problema o la tarea en una frase
- **Descripción**: contexto, pasos para reproducir el problema (si es un bug), o criterios de aceptación (si es una tarea)
- **Labels**: etiquetas para clasificarlo (bug, enhancement, documentation, question...)
- **Assignee**: quién se encarga de resolverlo
- **Milestone**: a qué hito o versión está asociado (opcional)

---

## Labels: organiza los issues

GitHub incluye labels predeterminados. Puedes crear los tuyos propios:

| Label | Uso habitual |
|---|---|
| `bug` | Algo que no funciona como debería |
| `enhancement` | Mejora o nueva funcionalidad |
| `documentation` | Relacionado con la documentación |
| `question` | Duda o pregunta |
| `good first issue` | Apto para contribuidores nuevos |
| `help wanted` | Se busca ayuda de la comunidad |

---

## Issues y commits: la conexión

Puedes referenciar un issue desde un commit mencionando su número:

```
fix: corregir calculo de fechas

Cierra el issue #12 reportado por el usuario.
```

Cuando ese commit llega a la rama principal, GitHub cierra automáticamente el issue `#12`.

Palabras clave para cerrar automáticamente: `closes`, `fixes`, `resolves` seguido del número de issue (`#12`).

---

## GitHub Projects: gestión visual del trabajo

**GitHub Projects** es una herramienta de planificación dentro de GitHub para organizar trabajo con vistas tipo **tabla**, **tablero** y, en algunos casos, **roadmap**. Puede conectarse con issues, pull requests y borradores de tareas.

Es especialmente útil para:
- Equipos de desarrollo que necesitan planificar sprints
- Proyectos personales con múltiples tareas en paralelo
- Docentes que gestionan el progreso de un grupo
- Repositorios donde conviene ver de un vistazo qué está pendiente, qué está bloqueado y qué ya se terminó

Lo importante no es solo "tener un tablero", sino usarlo como una fuente de verdad sobre el estado real del trabajo.

---

## Cómo pensar un Project de forma útil

Un Project funciona mejor cuando cada tarjeta representa una tarea concreta y visible. Normalmente esa tarjeta será un **issue**, no una idea vaga.

Una organización simple y efectiva puede ser:

| Estado | Significado |
|---|---|
| `Todo` | Aún no se ha empezado |
| `In Progress` | Alguien está trabajando activamente en ello |
| `Blocked` | No puede avanzar por una dependencia o problema |
| `Done` | Ya está terminado |

Si el proyecto es pequeño, estas cuatro columnas suelen ser suficientes. Añadir demasiados estados complica más de lo que ayuda.

---

## Qué conviene meter en un Project

Mete en el Project tareas que realmente necesiten seguimiento:

- Issues de bugs
- Mejoras o nuevas funcionalidades
- Tareas de documentación
- Trabajo técnico pendiente
- Borradores de tareas todavía no convertidas en issue

No metas cualquier cosa. Si una tarea se resuelve en dos minutos y no necesita seguimiento, probablemente no hace falta convertirla en tarjeta.

---

## Flujo recomendado de trabajo

Una forma sana de trabajar con issues y Projects es esta:

1. Detectas una necesidad o problema
2. Creas un issue con título, contexto y criterio de cierre
3. Lo etiquetas (`bug`, `documentation`, `enhancement`...)
4. Lo añades al Project
5. Lo mueves a `In Progress` cuando realmente empiezas
6. Trabajas en una rama relacionada
7. Abres un pull request enlazado con ese issue
8. Cuando se mergea, marcas o dejas que GitHub marque la tarea como terminada

Este flujo evita dos errores muy comunes:
- Empezar trabajo sin dejar rastro de por qué se está haciendo
- Tener un tablero desactualizado que no refleja la realidad

---

## Consejos para organizar bien las tareas

- Escribe issues pequeños y accionables. "Mejorar la app" no sirve; "Añadir validación al formulario de registro" sí.
- Usa títulos que empiecen con un verbo: `Corregir`, `Añadir`, `Actualizar`, `Documentar`.
- No tengas demasiadas tareas en `In Progress`. Si todo está en curso, en realidad no sabes qué es prioritario.
- Usa labels para clasificar, no para decorar. Si una etiqueta no ayuda a filtrar o decidir, sobra.
- Revisa el Project con frecuencia. Un tablero que no se mantiene acaba perdiendo valor.
- Añade criterio de cierre en las tareas importantes: ¿qué tiene que pasar para considerarla terminada?
- Separa trabajo grande en varias tareas pequeñas. Un issue enorme es difícil de estimar, asignar y cerrar.
- Si una tarea depende de otra, indícalo en la descripción para evitar bloqueos invisibles.

---

## Errores habituales

- Usar Projects como lista decorativa y no actualizar estados
- Abrir issues sin contexto suficiente
- Mezclar en una sola tarea varias cosas no relacionadas
- Cerrar tareas porque "casi están" en lugar de porque realmente cumplen su objetivo
- Tener más columnas y etiquetas de las que el equipo puede mantener

---

## Cuándo merece la pena usarlo

En un proyecto muy pequeño quizá baste con unos pocos issues. Pero en cuanto hay varias tareas abiertas, colaboración con otras personas o trabajo que se extiende durante varios días, un Project empieza a aportar claridad real.

Se configura desde la interfaz web de GitHub, en la pestaña **Projects** del repositorio o desde tu perfil.
