# Ejercicio — Commits bien escritos

## Parte 1: Diagnóstico de mensajes

Lee estos mensajes de commit e identifica cuáles son buenos y cuáles no. Para los malos, propón una versión mejorada siguiendo la convención.

```
1. cambios varios
2. feat: agregar campo de telefono al formulario de contacto
3. fix bug
4. docs: corregir enlace roto en README
5. actualizar
6. refactor: simplificar logica de validacion de fechas
7. wip esto no funciona todavia
8. chore: actualizar .gitignore para ignorar archivos .env
```

---

## Parte 2: Practica en tu repositorio

En tu carpeta `practica-git`, crea un archivo llamado `aprendizajes.md` con este contenido:

```markdown
# Aprendizajes

## Commits
- Los mensajes deben explicar qué y por qué
- La convención es: tipo: descripción breve
```

Ahora haz el commit con un buen mensaje:

```bash
git add aprendizajes.md
git commit -m "docs: agregar lista de aprendizajes sobre commits"
```

---

## Parte 3: Commit con cuerpo largo

Modifica `aprendizajes.md` añadiendo una sección nueva. Luego haz un commit **abriendo el editor**:

```bash
git add aprendizajes.md
git commit
```

Escribe un título en la primera línea, deja una línea en blanco y añade en el cuerpo el motivo del cambio. Guarda y cierra el editor.

Verifica el resultado:

```bash
git log
```

---

## Parte 4: Revisa tus commits anteriores

Ejecuta:

```bash
git log --oneline
```

Mira todos los commits que has hecho hasta ahora. ¿Alguno tiene un mensaje que no seguiría la convención? Si el más reciente se puede mejorar:

```bash
git commit --amend -m "tipo: mensaje mejorado"
```

---

## Resultado esperado

- Puedes distinguir un buen mensaje de commit de uno malo
- Tus últimos commits siguen la convención `tipo: descripción`
- Has probado a escribir un commit con cuerpo largo usando el editor
