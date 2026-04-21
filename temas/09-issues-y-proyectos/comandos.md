# Comandos — Issues y Proyectos

Los issues y proyectos se gestionan principalmente desde la interfaz web de GitHub. No requieren comandos de terminal.

Sin embargo, hay formas de conectarlos con tu trabajo en la terminal:

---

## Referenciar issues en commits

```bash
# Mencionar un issue en el mensaje de commit
git commit -m "fix: corregir error en calculo

Relacionado con el issue #5."

# Cerrar un issue automáticamente al hacer merge a main
git commit -m "fix: corregir calculo de descuentos

Closes #5."
```

Las palabras clave que cierran un issue automáticamente son:
- `closes #N`
- `fixes #N`
- `resolves #N`

---

## GitHub CLI (opcional, para usuarios avanzados)

Si instalas la herramienta `gh` ([cli.github.com](https://cli.github.com)), puedes gestionar issues desde la terminal:

```bash
# Ver los issues abiertos
gh issue list

# Crear un issue
gh issue create --title "Bug en formulario" --body "Descripción del problema"

# Ver un issue concreto
gh issue view 5
```

> Esto es completamente opcional. Todo lo que hace `gh` también se puede hacer desde la web.

---

## GitHub Projects con GitHub CLI (avanzado)

GitHub Projects se usa sobre todo desde la web, pero `gh` también permite automatizar parte del trabajo.

```bash
# Listar projects accesibles para tu usuario
gh project list --owner TU-USUARIO

# Crear un project nuevo
gh project create --owner TU-USUARIO --title "Tareas practica-git"

# Ver un project concreto
gh project view NUMERO --owner TU-USUARIO
```

En muchos casos, la forma más cómoda sigue siendo la interfaz web, sobre todo para mover tareas entre estados y configurar campos.

---

## Consejo práctico de uso

Aunque puedas usar CLI, el flujo más claro para aprender suele ser:

1. Crear el issue desde la web
2. Añadirlo al Project
3. Trabajar en local con Git
4. Referenciar el issue en commits o en el pull request
5. Volver al Project para actualizar el estado real

La terminal te ayuda a desarrollar; el Project te ayuda a no perder el control del trabajo.
