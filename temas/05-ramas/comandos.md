# Comandos — Ramas

## Crear y navegar entre ramas

```bash
# Ver las ramas locales (la activa tiene un *)
git branch

# Ver todas las ramas (locales y remotas)
git branch -a

# Crear una nueva rama y cambiarte a ella
git switch -c nombre-de-la-rama

# Cambiarte a una rama que ya existe
git switch nombre-de-la-rama

# Forma antigua (equivalente a switch -c)
git checkout -b nombre-de-la-rama
```

---

## Gestionar ramas

```bash
# Renombrar la rama actual
git branch -m nuevo-nombre

# Eliminar una rama (solo si ya fue fusionada)
git branch -d nombre-de-la-rama

# Eliminar forzosamente (aunque no esté fusionada)
git branch -D nombre-de-la-rama
```

---

## Comprobar en qué punto está cada rama

```bash
# Ver el historial con las ramas representadas gráficamente
git log --oneline --graph --all
```

Este comando es muy útil para visualizar dónde está cada rama en el historial.

---

## Guardar trabajo a medias (stash)

```bash
# Guardar los cambios actuales sin commitear (limpia el working directory)
git stash

# Ver los cambios guardados en el stash
git stash list

# Recuperar el último stash y aplicarlo al working directory
git stash pop

# Recuperar sin eliminarlo del stash (por si quieres aplicarlo en varias ramas)
git stash apply

# Eliminar el stash sin aplicarlo
git stash drop
```
