# Comandos — Commits bien escritos

## Hacer un commit

```bash
# Con mensaje corto en línea
git commit -m "tipo: descripción breve"

# Abriendo el editor para escribir mensaje largo
git commit
```

---

## Ver el historial

```bash
# Historial compacto
git log --oneline

# Historial completo con cuerpo de mensaje
git log

# Ver los cambios incluidos en cada commit
git log -p

# Ver estadísticas de cambios por commit
git log --stat
```

---

## Modificar el último commit

```bash
# Cambiar el mensaje del último commit (solo si no lo has publicado)
git commit --amend -m "tipo: nuevo mensaje corregido"

# Añadir un archivo olvidado al último commit
git add archivo-olvidado.md
git commit --amend --no-edit
```

> ⚠️ Usa `--amend` solo en commits que **no has compartido** todavía con nadie. Modificar commits publicados puede causar problemas a otras personas.

---

## Ver un commit concreto

```bash
# Ver los cambios de un commit específico (usa su identificador del log)
git show abc1234
```

---

## Deshacer commits

```bash
# Deshace el último commit, conserva los cambios en staging
# (útil para reescribir el mensaje o ajustar qué incluye el commit)
git reset --soft HEAD~1

# Deshace el último commit, vuelve los cambios al working directory
git reset HEAD~1

# Crea un commit nuevo que revierte los cambios de un commit ya publicado
# (la forma segura cuando el commit ya está en el remoto)
git revert abc1234
```

> Usa `reset` solo en commits que no has compartido con nadie. Usa `revert` cuando el commit ya está publicado en GitHub.
