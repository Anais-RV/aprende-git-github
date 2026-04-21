# Ejercicio — El ciclo básico

Usarás la carpeta `practica-git` que creaste en el tema anterior.

---

## Paso 1: Crea tu primer archivo de contenido

Dentro de `practica-git`, crea un archivo llamado `notas.md` con este contenido:

```markdown
# Mis notas de Git

## Lo que estoy aprendiendo

- Git guarda instantáneas del proyecto llamadas commits
- El ciclo básico es: editar → add → commit
```

---

## Paso 2: Comprueba el estado

```bash
git status
```

Deberías ver `notas.md` en rojo como archivo "untracked" (no rastreado).

---

## Paso 3: Añade el archivo al staging

```bash
git add notas.md
```

Vuelve a ejecutar `git status`. Ahora el archivo aparece en verde bajo "Changes to be committed".

---

## Paso 4: Haz tu primer commit

```bash
git commit -m "docs: agregar notas iniciales sobre git"
```

---

## Paso 5: Consulta el historial

```bash
git log --oneline
```

Deberías ver tu commit listado con su identificador corto y el mensaje.

---

## Paso 6: Modifica y repite el ciclo

Abre `notas.md` y añade una línea nueva:

```markdown
- La staging area me permite elegir qué va en cada commit
```

Guarda el archivo, y repite el ciclo:

```bash
git status
git add notas.md
git commit -m "docs: agregar nota sobre staging area"
git log --oneline
```

---

## Paso 7: Practica `git diff`

Modifica `notas.md` pero **antes de hacer `git add`**, ejecuta:

```bash
git diff
```

Observa cómo te muestra exactamente qué líneas cambiaron (en rojo las borradas, en verde las añadidas).

---

## Resultado esperado

- Tienes al menos 2 commits en tu repositorio de práctica
- Entiendes la diferencia entre working directory, staging y el repositorio
- Puedes leer la salida de `git status` y `git log --oneline` sin ayuda
