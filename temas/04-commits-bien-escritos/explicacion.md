# Commits bien escritos

## ¿Por qué importa el mensaje de un commit?

El código cambia, los archivos cambian, los proyectos evolucionan. El historial de commits es la única documentación que siempre está actualizada sobre cómo llegaste al estado actual.

Un mensaje de commit malo:
```
cambios
wip
arreglado
commit
final v2
```

Un mensaje de commit bueno:
```
fix: corregir formula de calculo de impuestos en checkout
feat: agregar validacion de email en formulario de registro
docs: actualizar instrucciones de instalacion para Windows
```

La diferencia no es estética. Es práctica: dentro de tres meses, cuando busques en el historial por qué cambió algo, los mensajes claros te ahorran horas de trabajo.

---

## La pregunta que debes hacerte

Antes de escribir un mensaje, completa esta frase mentalmente:

> "Si aplico este commit, este commit va a **___**."

Ese hueco es tu mensaje de commit.

- ❌ "cambios en login" → no dice qué cambió ni por qué
- ✅ "fix: corregir error que bloqueaba el login con email en mayusculas"

---

## Conventional Commits (versión simplificada)

Esta convención añade un **prefijo de tipo** al mensaje para clasificar los commits:

```
tipo: descripción breve en imperativo y minúsculas
```

| Tipo | Significado |
|---|---|
| `feat` | Nueva funcionalidad o contenido |
| `fix` | Corrección de un error |
| `docs` | Cambios solo en documentación |
| `refactor` | Mejora interna sin cambiar lo que hace |
| `chore` | Tareas de mantenimiento (gitignore, config...) |

Consulta el archivo [CONVENCIONES.md](CONVENCIONES.md) para más detalles y ejemplos.

---

## El qué vs el por qué

Los mensajes de commit cortos explican **qué** hiciste. Pero a veces igual de importante es **por qué**.

Para esos casos, puedes añadir una descripción larga al commit:

```bash
git commit
```

Esto abre tu editor. La primera línea es el título (corto). Después de una línea en blanco, puedes escribir el cuerpo del mensaje con todo el contexto que necesites.

```
fix: corregir calculo de fecha de vencimiento

El calculo anterior no tenia en cuenta los años bisiestos,
lo que causaba que los recordatorios llegaran un dia tarde
en febrero de años bisiestos. Se cambia la libreria usada.
```

---

## Regla de oro

Un buen historial de commits cuenta la historia de tu proyecto. Si alguien lo lee de arriba a abajo, debería entender cómo y por qué evolucionó.

---

## Deshacer commits: cuándo y cómo

Cometemos errores. Publicamos un commit con un mensaje malo, incluimos algo que no debía ir, o simplemente cambiamos de idea. Git tiene herramientas para cada situación.

### Si el commit no está publicado todavía (solo en local)

```bash
# Deshace el último commit pero conserva los cambios en staging
git reset --soft HEAD~1

# Deshace el último commit y vuelve los cambios al working directory
git reset HEAD~1
```

Usa esto para corregir el último commit antes de hacer push.

### Si el commit ya está publicado (en GitHub)

```bash
# Crea un nuevo commit que revierte los cambios del commit indicado
git revert abc1234
```

`git revert` no borra el commit original — añade uno nuevo que deshace los cambios. Es la forma segura de deshacer trabajo que ya has compartido, porque no reescribe el historial.

> La regla general: si el commit ya está en el remoto y otras personas pueden haberlo visto, usa `git revert`. Si todavía está solo en tu máquina, puedes usar `git reset`.
