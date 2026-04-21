# Ejercicio — Ramas

## Paso 1: Comprueba tu rama actual

En tu carpeta `practica-git`:

```bash
git branch
```

Deberías estar en `main`. Si aparece `master`, no te preocupes, es lo mismo en proyectos más antiguos.

---

## Paso 2: Crea una rama de experimento

```bash
git switch -c experimento/nueva-seccion
```

Verifica que cambiaste de rama:

```bash
git branch
```

---

## Paso 3: Haz cambios en la nueva rama

Abre `notas.md` y añade una sección nueva al final:

```markdown
## Ramas

- Las ramas permiten trabajar en paralelo
- La rama main es el estado oficial del proyecto
- Se pueden fusionar ramas con git merge
```

Guarda y haz el commit en esta rama:

```bash
git add notas.md
git commit -m "docs: agregar seccion sobre ramas en notas"
```

---

## Paso 4: Vuelve a main y comprueba

```bash
git switch main
```

Abre `notas.md`. La sección que acabas de escribir **no aparece** — eso es correcto. Está en la otra rama, no en `main`.

---

## Paso 5: Visualiza el estado de las ramas

```bash
git log --oneline --graph --all
```

Deberías ver las dos ramas divergiendo en el historial.

---

## Paso 6: Crea una segunda rama desde main

Sin salir de `main`:

```bash
git switch -c docs/mejora-aprendizajes
```

Añade una línea a `aprendizajes.md` y haz commit.

---

## Paso 7: Lista todas las ramas

```bash
git branch
```

Deberías tener al menos tres ramas: `main`, `experimento/nueva-seccion` y `docs/mejora-aprendizajes`.

---

## Resultado esperado

- Sabes crear ramas, cambiarte entre ellas y listarlas
- Entiendes que los cambios en una rama no afectan a las demás
- Puedes visualizar el historial de ramas con `git log --oneline --graph --all`
