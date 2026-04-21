# README y documentación

## El README: la primera impresión de tu proyecto

El archivo `README.md` es lo primero que ve alguien cuando llega a tu repositorio en GitHub. Es la portada, el manual y la tarjeta de presentación del proyecto, todo en uno.

Un README bien escrito responde a estas preguntas:
- ¿Qué es este proyecto?
- ¿Para qué sirve?
- ¿Cómo se instala o se usa?
- ¿Cómo puedo contribuir?

---

## Markdown: el lenguaje del README

Los archivos `.md` se escriben en **Markdown**, un lenguaje de marcado ligero que GitHub renderiza como HTML. Ya lo estás usando en este repositorio.

### Elementos más usados

```markdown
# Título grande (H1)
## Título mediano (H2)
### Título pequeño (H3)

**negrita**
*cursiva*
`código en línea`

- Elemento de lista
- Otro elemento

1. Lista numerada
2. Segundo elemento

[Texto del enlace](https://url.com)
![Texto alternativo](ruta/imagen.png)

> Cita o nota destacada

---   ← línea horizontal
```

### Bloques de código

````
```bash
git commit -m "tipo: descripción"
```
````

Especifica el lenguaje después de los tres backticks para que GitHub aplique el resaltado de sintaxis.

### Tablas

```markdown
| Columna 1 | Columna 2 | Columna 3 |
|---|---|---|
| Dato A | Dato B | Dato C |
```

---

## Estructura recomendada para un README

```markdown
# Nombre del Proyecto

Descripción breve en 1-2 frases.

## ¿Para qué sirve?

Explica el problema que resuelve.

## Instalación

Pasos concretos para poner en marcha el proyecto.

## Uso

Ejemplo básico de uso con código.

## Contribuir

Cómo puede alguien contribuir al proyecto.

## Licencia

Qué licencia tiene el proyecto.
```

No todos los proyectos necesitan todas las secciones. Adapta la estructura a lo que tu proyecto necesita.

---

## Buenas prácticas de documentación

- **Escribe para alguien que no sabe nada del contexto**: incluye todo lo necesario para que funcione
- **Mantén el README actualizado**: un README desactualizado es peor que no tener ninguno
- **Usa ejemplos reales**: un ejemplo de código vale más que un párrafo de explicación
- **Sé conciso**: los READMEs largos no se leen. Menos es más

---

## Otros archivos de documentación útiles

| Archivo | Propósito |
|---|---|
| `CONTRIBUTING.md` | Cómo contribuir al proyecto |
| `CHANGELOG.md` | Historial de cambios por versión |
| `LICENSE` | Licencia del proyecto |
| `CODE_OF_CONDUCT.md` | Normas de comportamiento para la comunidad |

GitHub los detecta automáticamente y los enlaza en la interfaz.
