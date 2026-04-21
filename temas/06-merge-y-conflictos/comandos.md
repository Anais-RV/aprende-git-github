# Comandos — Merge y conflictos

## Fusionar ramas

```bash
# Estando en la rama destino, incorporar otra rama
git merge nombre-de-la-rama

# Merge con mensaje de commit personalizado
git merge nombre-de-la-rama -m "merge: incorporar feature/nueva-seccion"

# Cancelar un merge en curso (vuelve al estado anterior)
git merge --abort
```

---

## Durante un conflicto

```bash
# Ver qué archivos tienen conflictos
git status

# Después de resolver manualmente los conflictos, marcar como resuelto
git add archivo-resuelto.md

# Ver los marcadores de conflicto desde la terminal
git diff
```

---

## Ver diferencias entre ramas

```bash
# Ver qué cambios tiene una rama respecto a otra
git diff main..nombre-de-la-rama

# Ver los commits que tiene una rama y la otra no
git log main..nombre-de-la-rama --oneline
```

---

## Limpiar ramas fusionadas

```bash
# Eliminar rama local ya fusionada
git branch -d nombre-de-la-rama

# Ver ramas que ya han sido fusionadas en la actual
git branch --merged

# Ver ramas que NO han sido fusionadas todavía
git branch --no-merged
```
