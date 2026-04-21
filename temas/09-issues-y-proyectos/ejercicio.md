# Ejercicio — Issues y Proyectos

## Parte 1: Crear y gestionar issues

### Paso 1: Abre tu repositorio en GitHub

Ve a `github.com/TU-USUARIO/practica-git` y haz clic en la pestaña **Issues**.

### Paso 2: Crea tres issues

Crea los siguientes issues (o similares adaptados a tu proyecto):

**Issue 1 — Mejora**
- Título: `Añadir sección de recursos adicionales a notas.md`
- Label: `enhancement`
- Descripción: "La sección de notas está bien pero podría incluir enlaces a recursos externos para profundizar."

**Issue 2 — Documentación**
- Título: `Mejorar la introducción en el README`
- Label: `documentation`
- Descripción: "El README no explica bien el propósito del repositorio para alguien que llega por primera vez."

**Issue 3 — Pregunta**
- Título: `¿Cuál es la diferencia entre git fetch y git pull?`
- Label: `question`
- Descripción: Escribe aquí tu duda real si tienes alguna, o formula una pregunta de práctica.

---

## Parte 2: Resuelve un issue con un commit

Elige el Issue 1 y resuélvelo:

1. En local, crea una rama para este trabajo:
   ```bash
   git switch -c feat/recursos-adicionales
   ```

2. Añade al final de `notas.md`:
   ```markdown
   ## Recursos adicionales

   - [Documentación oficial de Git](https://git-scm.com/doc)
   - [GitHub Docs](https://docs.github.com)
   - [Pro Git (libro gratuito)](https://git-scm.com/book/es/v2)
   ```

3. Haz commit mencionando el issue (usa el número real que GitHub le asignó):
   ```bash
   git add notas.md
   git commit -m "feat: agregar seccion de recursos adicionales

   Closes #1."
   ```

4. Haz push y abre un PR. Cuando el PR se mergee a main, el issue se cerrará automáticamente.

---

## Parte 3: Crea un Project (tablero)

1. Ve a la pestaña **Projects** de tu repositorio
2. Haz clic en **New project**
3. Elige el template **Board** (tablero kanban)
4. Dale un nombre: "Tareas practica-git"
5. Añade tus tres issues abiertos al tablero
6. Organízalos en las columnas: "Todo", "In Progress", "Blocked", "Done"

---

## Parte 4: Organiza el trabajo con criterio

Ahora mejora tu Project para que sea realmente útil:

1. Deja solo una tarea en `In Progress`
2. Mueve a `Blocked` cualquier tarea que no puedas completar todavía
3. Revisa los títulos de los issues y hazlos más concretos si hace falta
4. Añade en al menos un issue una condición clara de cierre en la descripción
5. Decide cuál es la tarea más importante y colócala arriba en `Todo`

Si quieres ir un paso más allá, crea un issue adicional de documentación y añádelo al tablero.

---

## Resultado esperado

- Tienes al menos 3 issues creados con labels y descripciones claras
- Sabes conectar un commit con un issue para cerrarlo automáticamente
- Has creado un tablero de proyecto básico en GitHub
- Tu tablero refleja prioridades reales y no solo una lista de tareas
