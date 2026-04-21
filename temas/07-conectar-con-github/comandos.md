# Comandos — Conectar con GitHub

## Gestionar remotos

```bash
# Ver los remotos configurados
git remote -v

# Añadir un remoto
git remote add origin https://github.com/usuario/repo.git

# Cambiar la URL de un remoto
git remote set-url origin https://github.com/usuario/nuevo-repo.git

# Eliminar un remoto
git remote remove origin
```

---

## Enviar cambios al remoto (push)

```bash
# Primera vez: publicar la rama y configurar seguimiento
git push -u origin main

# Las veces siguientes (una vez configurado el seguimiento)
git push

# Enviar una rama específica
git push origin nombre-de-la-rama

# Enviar todas las ramas locales
git push --all
```

---

## Traer cambios del remoto (pull)

```bash
# Traer y fusionar cambios del remoto en la rama actual
git pull

# Traer cambios sin fusionar (para revisar antes)
git fetch

# Ver qué hay en el remoto sin aplicar nada
git fetch origin
git log origin/main --oneline
```

---

## Clonar un repositorio

```bash
# Clonar en una carpeta con el nombre del repositorio
git clone https://github.com/usuario/repo.git

# Clonar en una carpeta con nombre específico
git clone https://github.com/usuario/repo.git mi-carpeta
```

---

## Ver el estado respecto al remoto

```bash
# Ver commits locales que no están en el remoto
git log origin/main..HEAD --oneline

# Ver commits del remoto que no tienes en local
git log HEAD..origin/main --oneline
```
