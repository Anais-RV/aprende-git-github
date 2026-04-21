# Convenciones de commits

Una parte esencial de trabajar con Git es escribir mensajes de commit que tengan sentido, no solo para ti ahora, sino para cualquier persona (incluido tu yo futuro) que lea el historial dentro de seis meses.

---

## Formato

```
tipo: descripción breve en presente e imperativo
```

La descripción debe completar la frase: _"Si aplico este commit, este commit va a..."_

---

## Tipos de commit

| Tipo | Cuándo usarlo |
|---|---|
| `feat` | Añades algo nuevo (un archivo, una sección, una funcionalidad) |
| `fix` | Corriges un error o algo que estaba mal |
| `docs` | Cambios solo de documentación |
| `refactor` | Reorganizas o limpias sin cambiar lo que hace |
| `chore` | Tareas de mantenimiento (configuración, .gitignore, etc.) |

---

## Ejemplos

```
✅ feat: agregar explicacion del ciclo basico de git
✅ fix: corregir comando incorrecto en ejercicio de ramas
✅ docs: actualizar README con nuevo temario
✅ chore: agregar .gitignore para archivos de sistema

❌ cambios
❌ arreglado
❌ wip
❌ commit final definitivo v2
```

---

## Por qué importa

Un historial de commits bien escrito es una **documentación automática** de tu proyecto. Permite entender qué cambió, cuándo y por qué, sin tener que abrir cada archivo.

> Un commit es una decisión registrada, no un trámite.
