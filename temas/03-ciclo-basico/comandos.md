# Comandos — El ciclo básico

## Ver el estado del repositorio

```bash
git status
```

El comando más usado de todos. Muestra qué archivos están modificados, en staging o sin rastrear. Úsalo constantemente.

---

## Añadir archivos al staging

```bash
# Añadir un archivo concreto
git add archivo.md

# Añadir varios archivos
git add archivo1.md archivo2.md

# Añadir todos los cambios de la carpeta actual
git add .

# Añadir de forma interactiva (elige qué incluir)
git add -p
```

---

## Hacer un commit

```bash
# Commit con mensaje en línea
git commit -m "tipo: descripción breve"

# Commit abriendo el editor de texto para escribir el mensaje
git commit
```

---

## Ver el historial de commits

```bash
# Historial completo
git log

# Historial compacto (una línea por commit)
git log --oneline

# Historial con gráfico de ramas
git log --oneline --graph

# Ver los últimos N commits
git log -5
```

---

## Deshacer: sacar un archivo del staging

```bash
# Si añadiste un archivo por error antes de hacer commit
git restore --staged archivo.md
```

---

## Deshacer: descartar cambios en el working directory

```bash
# Vuelve el archivo a como estaba en el último commit
# ⚠️ Esto borra los cambios sin guardado previo — no tiene vuelta atrás
git restore archivo.md
```

---

## Ver qué cambió exactamente

```bash
# Cambios en el working directory (no en staging)
git diff

# Cambios que ya están en staging
git diff --staged
```
